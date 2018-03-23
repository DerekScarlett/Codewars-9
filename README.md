# Codewars-9
Question: Find the number with the most digits.
If two numbers in the argument array have the same number of digits, return the first one in the array.

Solution:
//wrote a function that takes in an array
function findLongest(array){
//made a variable to store the number that had the most digits
  var biggestNum = 0;
//this for loop , loops through my array of numbers
  for(var i = 0; i < array.length; i++) {
  //theres two conditions that need to be met
   //-the number needs to have the most diggest
   //- if two numbers have the same number of digits , return the first one in the array
    if(array[i].toString().length > biggestNum.toString().length) {
      biggestNum = array[i];
    }
  }
  //return your biggest number
  return biggestNum;
}
console.log(findLongest([111, 1111, 5555, 10000, 1, 90000]));
