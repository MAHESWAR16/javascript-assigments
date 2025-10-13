#                                                                               JAVASCRIPT FUNCTIONS

# What is a function?
A function is like a small box that can do some work for you.

Example 👇
function add() 
{
 console.log("I am adding numbers");
 }

 Here —
the box name is add,
and inside the box is the work: console.log("I am adding numbers").
 Step 2: How do we make the box work?
 We tell JavaScript:
“Hey, open the box and do the work!” We do that like this 👇
add();
Now it prints:
I am adding numbers


# Step 3: What if we want the box to open by itself?

Let’s say you want the box to open immediately —
the moment JavaScript sees it.
You can do this 👇
(function() {
 console.log("Box opened automatically!");
 })();

✅ Output:
Box opened automatically!
You didn’t say add(); anywhere.
It just ran by itself! 😄
  🪄 Step 4: How does it work?
# Let’s break it slowly 👇
(function()

{

console.log("Hello!");

}

 )();
 
🔹 Part 1: (function()

{ ... }
)
 This makes a small box (function).
 🔹 Part 2: () at the end
This tells JavaScript:
 “Now open the box and run it!”
 So —
✅ You make the box
✅ and open it immediately.

Step 5: Why do people do this?
 Imagine your school bag. 🎒
 You put your pencils and erasers inside it.
 If you zip it closed — nobody can touch your pencils. ✏️
 That’s what this does.

 (function()

 {

  var pencil = "I am safe inside the bag";

  console.log(pencil);

 }

 )();

# ✅ Output:
 I am safe inside the bag
 If you try to look outside the bag 👇
console.log(pencil); // ❌
You’ll get an error —
because the pencil is inside the bag, and you can’t see it outside.


 Step 6: The Name (Don’t Worry About It)
 This box that opens by itself is called:
 IIFE (Immediately Invoked Function Expression)
 But you don’t need to remember the name yet.
Just remember this 👇

🟢 “A function that runs automatically.”

# : Simple Picture (Imagine this)
# ┌────────────────────────┐

# │ (function(){            │

# │   console.log("Hi!");   │

# │ })();                   │

# └────────────────────────┘

#          ↓

# Creates a box 🟦
# Opens it immediately ⚡
# Prints “Hi!”

## Step 7: See It Together
 (function()
 {
  var name = "Mahesh";
  console.log("Hello", name);
}
)();
 ✅ Output: Hello Mahesh

It runs immediately and hides the variable name inside.

Step 1: What is a variable?
A variable is like a small box that holds some information.
Example 👇
var name = "Mahesh";
console.log(name);
✅ Output:
Mahesh
So here:
name → is the box name.
"Mahesh" → is the thing kept inside the box.
🧠 Step 2: What happens when we make it inside a function?
Example 👇
function greet() {
  var name = "Mahesh";
  console.log("Hello", name);
}
greet();
✅ Output:
Hello Mahesh
Now, the name box is inside the function.
It only exists while the function is running.
💡 Step 3: What happens if we try to use it outside?
function greet() {

  var name = "Mahesh";

  console.log("Hello", name);

}

greet();
console.log(name); // ❌
❌ This gives an error:
ReferenceError: name is not defined
Why?
Because the variable name was made inside the function’s room —
you can’t see it outside that room.
🏠 Step 4: Think of a house example
Imagine your name paper is inside your room.
You can see it only when you’re inside the room.
If you go outside, you can’t see it anymore.
Same for JavaScript 👇
Inside function	Outside function
Can see name ✅	Can’t see name ❌
🧩 Step 5: Now the same with IIFE
Here’s your IIFE example again:
(function() {
  var name = "Mahesh";
  console.log("Hello", name);
})();

✅ Output:
Hello Mahesh
But if you try this 👇
console.log(name);
❌ You get:
ReferenceError: name is not defined
Because that name variable is hidden inside that small bubble (the IIFE).
🎒 Step 6: Easy Example (Think like a school bag)
The IIFE is like a bag. 🎒
Whatever you put inside that bag stays inside.
(function() {

  var pencil = "✏️ Pencil";

  console.log("Inside the bag:", pencil);

})();
✅ Inside the bag:
Inside the bag: ✏️ Pencil
❌ Outside the bag:
console.log(pencil);
gives:
ReferenceError: pencil is not defined
Because your pencil is inside the bag — you zipped it closed. 🔒

✅ So in simple words:
When we say “it hides the variable inside,”
it means that variable lives only inside the function (or IIFE)
and you can’t use it outside that function.
