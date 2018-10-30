# reverseArrayInPlace

let reverseArrayInPlace = (array) => {
// takes a vector and reverses it
   for (let i = Math.floor((array.length/2)-1); i >= 0; i--){
        let hold = array[i]
        array[i] = array[array.length -1 -i]
        array[array.length -1 -i] = hold 
   }
   return array
}
let value = [1,2,3,4,5]
console.log(reverseArrayInPlace(value))
//-> [5,4,3,2,1]
