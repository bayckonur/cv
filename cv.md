# __Aliaksandr Baiko__

## Contact:
- __Location:__ Poland, Warsaw;
- __Phone number:__ +48791739475;
- __For email contact:__ bayckonur@gmail.com;
- __GitHub:__ [bayckonur](https://github.com/bayckonur).

## __About me__:
I enrolled in the Belarusian State Technological University for mechatronic systems but soon realized it wasn't aligned with my long-term aspirations. I made the decision to leave and ventured into Front-End Development, where I am now exploring my passion and pursuing a career.

## __Skills:__
- __HTML__;
- __CSS__;
- __JavaScript__ (Basic);
- __Git__.
- __Api__.
- __AMPS, WAMP and MAMP__.
- __Wordpress__.

## __Code:__

```
"use strict";

const ticketPriceElement = document.getElementById('ticketPrice');
const baggagePriceElement = document.getElementById('baggagePrice');
const checkbox = document.getElementById('checkbox');

const initialTicketPrice = getNumericPrice(ticketPriceElement); 
const initialBaggagePrice = getNumericPrice(baggagePriceElement);


function getNumericPrice(element) {
    const text = element.textContent;
    return parseFloat(text.replace(/[^\d.-]/g, ''));
}


checkbox.addEventListener('change', function() {
    let numTicketPrice = getNumericPrice(ticketPriceElement); 
    let numBaggagePrice = getNumericPrice(baggagePriceElement);

    if (checkbox.checked) {
        let countPrice = numBaggagePrice + numTicketPrice;
        ticketPriceElement.textContent = `${countPrice} €`;
        baggagePriceElement.textContent = 'включен'; 
        baggagePriceElement.style.color = 'black'; 
    } else {
        ticketPriceElement.textContent = `${initialTicketPrice} €`;
        baggagePriceElement.textContent = `+ ${initialBaggagePrice} €`;
        baggagePriceElement.style.color = '#0c73fe';
    }
});
```
## __Experience:__
.....

## __Education:__ 
- __University:__ Belarusian National Technical University, Mechatronic systems - Unfinished higher education;
- __Courses:__ RS School JS/FE Pre-School 2024Q2.

## __Languages__
- __English:__ B1.
- __Russian:__ Native speaker.
