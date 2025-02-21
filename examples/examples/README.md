# JavaScript Best Practices - Examples  

var name = "Ali";
var name = "Reza"; // 
console.log(name); // "Reza"

const age = 25;
// age = 30; // ❌ Error: Assignment to constant variable.

let city = "Tehran";
city = "Mashhad"; // ✅ valid
console.log(city); // "Mashhad"

const numbers = [1, 2, 3];
const doubled = [];
numbers.forEach((num) => {
  doubled.push(num * 2);
});
console.log(doubled); // [2, 4, 6]

const doubledNumbers = numbers.map((num) => num * 2);
console.log(doubledNumbers); // [2, 4, 6]


const user = {};
console.log(user.profile.name); // ❌ TypeError

console.log(user.profile?.name); // ✅ it would not be undefined 
