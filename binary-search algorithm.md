[[Graph and Networking Algoriithms]]

### Binary-search to find the desired item in an array.
The array is always halved to find the item. 

let arr = [0, 2, 3, 4, 5, 6, 7, 8, 9, 11];
const binarysearch = (val, arr) => {
 let lower = arr[0];
 let upper = arr[arr.length - 1];
 while (lower <= upper) {
 const mid = lower + Math.floor((upper - lower) / 2);
 if (val === arr[mid]) {
 return mid;
 }
 if (val < arr[mid]) {
 upper = mid - 1;
 } else {
 lower = mid + 1;
 }
 }
 return -1;
};
console.log(binarysearch(6, arr));


#algorithms 