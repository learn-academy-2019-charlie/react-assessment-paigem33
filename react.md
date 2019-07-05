# React Assessments

Try your best to answer each question on your own before looking up the answer online. Once you're done writing your first answer, you can google the question and write the best answer you find.

#### 1. Here is a list of pros and cons to using the React library to build your application -- but some of them are false. Remove the false statements from the list:


- React is a modern, efficient answer to complex UI applications
- React is a flexible library that plays the role of V in an MVC framework

 
 #### 2. What are "smart"(logic) and "dumb"(display) components? Explain the difference and also add why we bother to make the distinction between them.
 
 
 //Your Answer
 
 Smart components are components that house state, while dumb components do not have their own state. Smart Components are where you will be writting logic, while dumb components are mostly for display.
 
 //Googled Answer
 
 Dumb components are also called ‘presentational’ components because their only responsibility is to present something to the DOM.
 
 Smart components (or container components) on the other hand have a different responsibility. Because they have the burden of being smart, they are the ones that keep track of state and care about how the app works.
 
#### 3. When we use "yarn add ..." in the terminal - what is yarn doing? And what file will always be automatically updated after we add a package with yarn?
 
 
 //Your Answer
 
 
 //Googled Answer
 
 In general, a package is simply a folder with code and a package.json file that describes the contents. When you want to use another package, you first need to add it to your dependencies. This means running yarn add [package-name] to install it into your project.
 Most packages will be installed from the npm registry and referred to by simply their package name. For example, yarn add react will install the react package from the npm registry.
 
#### 5. There are three mistakes in this code that would cause it to break our application. Find the mistakes and fix them:
cant use map on the recipes since it is not an array, map would need to be in the render not the render
    import React, { Component } from 'react';

    class Recipes extends Component*(1) {
      constructor(props){
        super(props)
        this.state = {
          recipes: 
            {name: 'Meatballs'},
            {name: 'Mac & Cheese'}
      
        }
      }

      render() {
    
        return (
        <div>
          let { recipes }*2 = this.state.recipes.map(function(recipe){
            return(
              <li key={recipe.name}>{recipe.name}</li>
            )
          })
    
          <ul>
            {recipes}
          </ul>
          </div>*3?
        );
      }
    }

    export default Recipes;

#### 6. Name three html input types. (NOTE: text is the default type - so it doesn't count in this case)
 
 //Your Answer
 
 number, submit, radio
 
 //Googled Answer
 
 <input type="number">
<input type="password">
<input type="radio">
 
 #### 7. How would you explain state to a friend who doesn't know code?
 
 //Your Answer
 
 I would explain state as the value of something. It could be anything, color, a number, a word. And just like value, state can be changed. The state of a banana changes from green to yellow, etc. 
 
 //Googled Answer
 
 State is like temperature to water, by changing the state of the temperature, you are able to manipulate the state of the watwer between ice and regular water
 
 #### 8. What is the difference between component state and props? Your answer should include a short explanation of both.
 
 
 //Your Answer
 
 State is exactly that, it is the state of something at a given time. 
 Props are states that are being sent over to other components that don't actually hold that state. Props are used to have communication between components.
 
 //Googled Answer
 
  props (short for “properties”) and state are both plain JavaScript objects. While both hold information that influences the output of render, they are different in one important way: props get passed to the component (similar to function parameters) whereas state is managed within the component (similar to variables declared within a function).
   
#### 9. Write a paragraph or so about your experience with building tic-tac-toe. Some topics to start with might be: things you learned about yourself, concepts from React that stood out to you, something about pair programming (if you paired), or the experience of building something in code from scratch.

While making tic-tac-toe and the other react projects, I was really happy to finally have a grasp on the concepts and see them in action. The overall experience was okay, but it was the first time I was in a mob with someone who had a more domineering attitude and a much better understanding of the material. I learned that in the future I need to be better about voicing my need to figure things out and to think about things on my own without help sometimes in order to really understand what's going on. 
