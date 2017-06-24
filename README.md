## Scope, hoisting and compartmentalization

### Answer the following:
In you own words, explain the concepts of scope, hoisting, compartmentalization.

Scope:
Scope determines the accessibility of variables and other resources in areas of your code.

Hoisting:
Hoisting is a JavaScript mechanism where variables and function declarations are moved to the top of their scope before code execution.

Compartmentalization:
Compartmentalization basically means to write your code so that it is protected from people who don't need to see it.It alsomakes your code clean and easier to maintain.

### Provide examples for all three, below:

#### Scope:

<!--var make is in global scope -->
var make = "Toyota";

function printMake() {

<!-- var otherMake is in the local scope -->
  var otherMake = "Hyundai";

  console.log(make);
}

printMake();


#### Hoisting:
<!-- var not hoisted -->
function roll(){

    bun();

    var bun = function(){};
}
roll();
<!-- var hoisted -->
function roll(){

    var bun;

    bun();

    bun = function(){};
}

roll();

#### Compartmentalization:
