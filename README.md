
# AddToCart

This is a firebase application that I created with the help of the tutorials on scrimba.


## Table of contents

 - [Source](/#Sources)
 - [Technology](/#Technology)
 - [Screenshot](/#Screenshot)
 - [What I learnt](/#WhatILearnt)
 - [Code Reference](/#codeReference)



## Sources
Project was created with the help of the amazing teachers at scrimba in the [Learn Firebase Course](https://scrimba.com/learn/firebase), you can follow along.

## Technology/Programs

- HTML
- CSS
- JavaScript
- Firebase 


## Screenshots

!["How will it look"](/assets/project-screenshot.png)


## What I learn

#### Key takeaways:
-Arrays are an important part of any web app of project better start digging deep into them. In this project, we had many examples of arrays. See below:


<code>
 onValue(shoppingListInDB, function(snapshot) {
    if (snapshot.exists()) {
        let itemsArray = Object.entries(snapshot.val())
    
        clearShoppingListEl()
        
        for (let i = 0; i < itemsArray.length; i++) {
            let currentItem = itemsArray[i]
            let currentItemID = currentItem[0]
            let currentItemValue = currentItem[1]
            
            appendItemToShoppingListEl(currentItem)
        }    
    } else {
        shoppingListEl.innerHTML = "If is blank you don't need anything..."
    }
})
</code>

## Deployment
I deployed by website by using [Netlify](https://addtocart-app-bygenn.netlify.app/)

## Scrimba
- [Their courses](https://scrimba.com/allcourses)
- [The Frontend Career Path](https://scrimba.com/learn/frontend)

