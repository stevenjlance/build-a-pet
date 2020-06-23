# BUILD A PET
-------------------
Congratulations! You've just adopted a brand new bunny!

![Bun](https://media.giphy.com/media/3oz8xHsoGJwIzvSNGM/giphy.gif)

This project is inspired by the [poke the bunny](https://youtu.be/MiVEvAQOV4U?t=8) game from an earlier internet era. You can see a preview of our version [here](https://build-a-pet-exemplar-apcsp.glitch.me).

GOAL
=========
Your goal is to build a Pet the Bunny (or anminal of your choice) app that takes in (1) the name of your animal and (2) how old they are. When you pet or feed the button, the message and/or image change as a result
![](https://media.giphy.com/media/cPN85BCDqkRZkLD8Kd/giphy.gif)

TASKS
=========
For today's lab you should do the following:
1. Pick an animal of your choosing and find both a happy and grumpy picture of it. Add them both to the `img` directory of this project, and then modify the index.html to show your animal instead of the bunny. You can keep the bunny if you want, but it's more fun to customize it. There is a pug in the folder if you are more of a dog person.
1. Create a pets variable that will track the number of pets. It should be initalized to look like:
```javascript
var pets = 0;
```
3. Get the information that the user puts into the form for the name and age. You should store this information in variables using `document.querySelector`.
4. Store the information for both the pet and feed buttons using `document.querySelector`.
5. Add an event listener to both the pet and feed buttons for a click event.
6. When the button is clicked, the variables should be updated with the information needed from the form.
**NOTE**: To get the value from a text input field you need to use `.value` with `.document.querySelector()`. For example, to get the value from the age of the animal
```javascript
age = document.querySelector("#ageInput").value;
```
7. The number of pets should **increase** by 1 when you click the pet button and it should print a message telling you how many pets the animal has had.
8. Make the animal image switch out for the cranky version when it gets more than its preferred number of pats. If the animal is under the age of 20 then it should be grumpy after 10 pets. If the animal is over the age of 20, it should become grumpy after 20 pets. **NOTE:** if you have a `querySelector()` for the imapgaea, then you can update images using `img.src=IMAGE LOCATION` the same way you would setup for other properties.
9. The animal gets happier as you feed it. Decrease the number of pets everytime you click the feed button.

EXTENSIONS
============
Once that's working, you have so many ways to make this project really cool! Here are some of the ways our students have changed this in the past.
* Make the animal's number of preferred pats random each time the page is loaded.
* Make several different levels of anger - and progress through them as you pet the animal more and more.
* Make the message slightly more responsive - maybe a warning when you start getting close to too many pats.
* Make other buttons like "sleep" and "play" and have the image change to a super happy pet if you take perfect care of your pet.
