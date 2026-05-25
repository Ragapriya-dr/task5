// Task 1
let frontEnd = ["HTML","CSS"];
let backEnd = ["Node","MongoDB"];

let merged = [...frontEnd,...backEnd];
console.log(merged);


// Task 2
let original = [1,2,3];

let copy = [...original];
copy.push(4);

console.log(original);
console.log(copy);


// Task 3
let student1 = {name:"Rahul"};
let student2 = {role:"Developer"};

let result = {...student1,...student2};

console.log(result);


// Task 4
function total(a,b,...rest){
  console.log(a);
  console.log(b);
  console.log(rest);
  console.log(rest.length);
}

total(1,2,3,4,5,6,7,8);


// Task 5
let colors = ["red","green","blue","yellow"];

let [r,g,b,y] = colors;

console.log(b);


// Task 6
let data = [1,[2,[3,[4]]]];

let [a,[b1,[c,[d]]]] = data;

console.log(a,b1,c,d);


// Task 7
let mobile = {
  brand:"Samsung",
  price:20000,
  color:"black"
};

let {brand,color} = mobile;

console.log(brand,color);


// Task 8
let numbers = [1,2,3];

numbers.push(4,5,6);
numbers.pop();

console.log(numbers);


// Task 9
let fruits = ["banana","orange"];

fruits.unshift("apple");
fruits.shift();

console.log(fruits);


// Task 10
let arr = [1,2,30,40,5,6];

arr.splice(2,2,3,4);

console.log(arr);


// Task 11
let a1 = [1,2];
let b2 = [3,4];

let ans = a1.concat(b2,5,6);

console.log(ans);


// Task 12
let marks = [10,20,30,40,50,60];

console.log(marks.slice(2,5));


// Task 13
let nest = [1,[2,[3,[4,[5]]]]];

console.log(nest.flat(Infinity));


// Task 14
let arr2 = [1,2,3,4,5];

arr2.fill("done",3);

console.log(arr2);


// Task 15
let values = [10,20,30,40];

console.log(values.includes(20));
console.log(values.includes(100));


// Task 16
let arr3 = [1,2,3,4,3,2];

console.log(arr3.indexOf(3));
console.log(arr3.indexOf(2));


// Task 17
console.log(arr3.lastIndexOf(3));
console.log(arr3.lastIndexOf(2));


// Task 18
let nums = [100,2,55,1,9];

console.log(nums.sort());

console.log(nums.sort((a,b)=>a-b));


// Task 19
let letters = ["a","b","c","d"];

console.log(letters.reverse());


// Task 20
let students = ["Rahul","Ajay","Kumar"];

students.push("Vijay");
students.splice(1,1);
students[1] = "Arun";
students.reverse();

console.log(students);


// Task 21
let cart = ["Shoes","Watch","Phone"];

cart.push("Laptop");
cart.splice(1,1);

console.log(cart.includes("Phone"));
console.log(cart.length);


// Task 22
let employee = {
  name:"Naveen",
  role:"Web Developer",
  salary:"5LPA"
};

let {name,role,salary} = employee;

console.log(name,role,salary);

let emp2 = {...employee};

emp2.salary = "8LPA";

console.log(employee);
console.log(emp2);


// Task 23
function company(name,...skills){
  console.log(name);
  console.log(skills);
  console.log(skills.length);
}

company("Naveen","HTML","CSS","JS","React");


// Task 24
let data1 = [1,2,3,4,5,6,7,8,9,10];

console.log(data1.slice(0,5));
console.log(data1.reverse());
console.log(data1.includes(7));
console.log(data1.indexOf(10));


// Task 25
let users = [
  {name:"Rahul",role:"Developer"},
  {name:"Ajay",role:"Designer"},
  {name:"Kumar",role:"Tester"}
];

users.push({name:"Vijay",role:"Manager"});

users.pop();

let extra = [
  {name:"Arun",role:"HR"},
  {name:"Siva",role:"Support"}
];

users = [...users,...extra];

users.forEach(user=>{
  console.log(user.name);
});

console.log(users.reverse());
