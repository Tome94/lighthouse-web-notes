### tips 
If a if statement is within a loop the boolean value will change depending on the index e.g
index1 can be true or false -> index 2 can be true or false
```javascript 
const eqArrays = function(array1, array2) {
  for (let i = 0; i < array1.length; i++){
    if (array1[i] ===array2[i]){
      return true
    }
    else {
      return false
    }
  }
}
  ```
  however if you want the statement be either true or false have the function return true and use if statement to return false
``` javascript
const eqArrays = function(array1, array2) {
  for (let i = 0; i < array1.length; i++) {
    if (array1[i] !== array2[i]) {
      return false;
    }
  }
  return true;
};
```