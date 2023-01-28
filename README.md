# Recursive-functions

function countEvenNumbers (arr) {
 // Sentinel value. Recursion stops on empty array.
 if (arr.length < 1) {
 return 0;
 }
 // The shift() method removes the first element from an array
 // and returns that element. This method changes the length of the array.
 var value = arr.shift();
 // `value % 2 === 0` tests if the number is even or odd
 // If it's even we add one to the result of counting the remainder of
 // the array. If it's odd, we add zero to it.
 return ((value % 2 === 0) ? 1 : 0) + countEvens(arr);
}
