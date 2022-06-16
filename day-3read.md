# day-3read. Links
What does .map() return?

          it returns a new array

If I want to loop through an array and display each value in JSX, how do I do that in React?

         You loop through with .map() and return a <li> element for the items.

Each list item needs a unique ____.

         key

What is the purpose of a key?

        is a special string attribute you need this included when you create list of elements, they also help react identify which items have changed, added or removed.

-----------------------------------------

What is the spread operator?

             it is a spread syntax that uses 3 dots (...) that expands an iterable obj to list of arguments

List 4 things that the spread operator can do.

          it can spread an array into separate arguments, it can copy an array, it can be used in math functions, and adding a, item to a list.

Give an example of using the spread operator to combine two arrays.

const fruits = ['🍏','🍊','🍌','🍉','🍍']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
fruits[0] = '🍑'
console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍
Give an example of using the spread operator to add a new item to an array.

      ex.

      const fruit = ["mango", "apple", "pineapple"]

      const moreFruit = ["guava", "lulo", ...fruit]

      console.log(moreFruit) // ["mango", "apple", "pineapple", "guave", "lulo"

      

Give an example of using the spread operator to combine two objects into one.

const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂


In the video, what is the first step that the developer does to pass functions between components?

      Create function the function where ever the state it is you will change.

In your own words, what does the increment function do?

          it modifies the array by updating the count.

How can you pass a method from a parent component into a child component?

          you can pass the increment function inside the person object from the video. so in this example you would put the increment method inside of the person object. increment = {this.increment}/>

How does the child component invoke a method that was passed to it from a parent component?

this.props.increment(this.props.name) calls the method that exist in parent adn pass along the name.