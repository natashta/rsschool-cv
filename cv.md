# Natalia Ryzhova
## Contacts
**E-mail:** natashta@gmail.com
**Telegramm:** @xrono

## Summary
My goal is to improve the javascript to get a job as a junior frontend developer. My strong point is html layout. I am familiar with and use vanilla Javascript in my work. I have experience as a freelance layout designer.

## Skills
* Html;
* CSS/Sass;
* Javascript;
* BEM metodology;
* Git;
* Figma.

## Example of latest code:
```
let addButton = document.querySelectorAll(".cards__button--add");
let removeButton = document.querySelectorAll(".cards__button--remove");
let cartCounter = document.querySelector(".cart__counter");

let counter = 0;

addButton.forEach(el => el.addEventListener("click", addToCart));
removeButton.forEach(el => el.addEventListener("click", removeFromCart));

function addToCart(evt) {
    evt.preventDefault();
    var target = evt.target;
    var cardMarker = target.parentNode.querySelector(".cards__marker");
    var cardContent = target.parentNode.querySelector(".cards__content");
    var currentRemoveButton = target.parentNode.querySelector(".cards__button--remove");
   
    if (cardMarker.classList.contains("cards__marker--off")) {
        cardMarker.classList.remove("cards__marker--off");
      }
    cardContent.classList.add("cards__content--chosen");
    target.classList.add("cards__button--off");
    currentRemoveButton.classList.remove("cards__button--off");

    counter++;
    cartCounter.innerHTML = counter;
}

function removeFromCart(evt) {
    evt.preventDefault();
    if (counter <=0) {counter = 0;}

    var target = evt.target;
    var cardMarker = target.parentNode.querySelector(".cards__marker");
    var cardContent = target.parentNode.querySelector(".cards__content");
    var currentAddButton = target.parentNode.querySelector(".cards__button--add");
   
    cardMarker.classList.add("cards__marker--off");
    if (cardContent.classList.contains("cards__content--chosen")) {
        cardContent.classList.remove("cards__content--chosen");
    }
    target.classList.add("cards__button--off");
    currentAddButton.classList.remove("cards__button--off");

    counter--;
    cartCounter.innerHTML = counter;
}
```

## Experience
I have experience in developing several commercial projects. You can find them here:
* [лендинг для инвестиционной компании ](https://natashta.github.io/invest_hero/index.html)
* [страница для рекламной акции](http://ruzik.ru/promo/2020.html)

## Online learning
 * Netology. Advanced HTML and CSS course, Advanced Javascript course
 * Htmlacademy.

## Language skills:
* Russian (native)
* English (advanced)
