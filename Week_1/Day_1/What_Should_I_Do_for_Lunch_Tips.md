### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```// Function, has a parameter of 2 variables, hungry (Boolean) and availableTime (integer)
const whatToDoForLunch = function(hungry, availableTime) {
  //First conditional statement, checks if the person is hungry
  if (hungry == true){

    // Frist condition, nested inside above condition, if the person has less than 20 minutes
    if (availableTime < 20){
      console.log('Grab a snack and get back to work')
    }
    // second condition, nested inside hungry condition, if the person has between 20 and 30 minutes
    else if (availableTime >= 20 && availableTime <= 30){
      console.log('Try a place near by!')
    }
    // else statement, no conditions needed to display if the person has more than 30 minutes.
    else {
      console.log('you are in a bootcamp, you should reconsider how much time you actually have to spare.')
    }

    // Else if statement for hungry, if it's false then they are not hungry.
  }
  else if (hungry == false){
    console.log('You are not hungry, get back to work')
  }
}
```