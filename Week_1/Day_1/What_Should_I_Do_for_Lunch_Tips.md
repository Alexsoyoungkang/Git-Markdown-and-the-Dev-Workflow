### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```JavaScript
const whatToDoForLunch = function(hungry, availableTime) {
  if (hungry === true) { // === true can be omitted since the argument is already there
    if (availableTime < 20) {
      console.log("Pick up a snack or grab something you have ready at home.");
    } else if (availableTime >= 20 && availableTime < 30) {
      console.log("You deserve a break and should take time to cook a tasty meal.");
    } else if (availableTime > 30) {
      console.log("This is an intense program after all and you should probably reconsider.");
    }
  } else {
    console.log("Wait until you're hungry");
  }
};
