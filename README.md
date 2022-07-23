# js-basics
function hello() {
  console.log("bret patterson");
}

function sayHello(name) {
  let lastName = "patterson";
  console.log("hello" + name + "" + lastName + "!!");
}
function sum(num1, num2) {
  console.log(num1 + num2);
  return num1 + num2;
}
function exec1() {
  for (let i = 0; i < 21; i++) {
    if (i != 7 && i != 13) {
      console.log(i);
    }
  }

  let name = "";

  if (!name) {
    console.error("name is required");
  }
}

function exce2() {
  let total = 0;
  let numbers = [123, 3, -1, 12, -123, 45, 10, 20, 203, -2, -29, 12, 123];
  for (let i = 0; i < numbers.length; i++) {
    let number = numbers[i];
    console.log(numbers);
    total = total + numbers;

    if (number < 0) {
      console.log("is negative", number);
    }
  }
}

function init() {
  console.log("intro page");

  hello();

  let myName = "bret";
  sayHello(myName);

  let res = sum(21, 21);
  console.log(res);

  exec1();
  exce2();
}

window.onload = init;
