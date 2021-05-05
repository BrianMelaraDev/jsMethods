map()
method that iterates through an array and executes a function to each iteration and returns a new array
ex.
let array = [2,3]
return array.map(x => x*3) // [6,9]
let array1 = [4,9,16]
return array1.map(Math.sqrt) // [2,3,4]
let array2 = [5,15,30]
function divide(givenNumber){
    return givenNumber / 5
}
return array2.map(divide) // [1,3,6]
Time Complexity - O(n) linear time complexity 




reduce()
executes a reducer function that takes in 4 possible parameters reduce((accumulator, currentValue, index, array) => { ... }, initialValue)
ex.
let array = [3,4,5,6]
return array.reduce(acc, curr) => acc + curr // 18
let array1 = [100,30,25]
return array1.reduce(acc,curr) => acc - curr // 45
let array2 = [1,2,3,4,5]
return array2.reduce(acc,curr) => acc + curr*2 // 29
Time Complexity - O(n) linear time complexity 

filter()
iterates though an array choosing any element that makes the function inside true
ex.
let string = ['apple','brian','door','cape','kite']
return string.filter(word => word.length > 4) // ['door','cape','kite']
return string.filter(word -> word.length > 5) // ['apple','brian']
let string1 = [15,18,21,34,15,16,12,17,19]
return string1.filter(age => age >= 18) // [18,21,34,19]
Time Complexity - O(n) linear time complexity 


forEach()
iterates through an array executing a callback to each one without creating a new array
ex.
let array = [2,4,6]
return array.forEach(number =>{
    return number * 2
}) // [4,8,12]
return array.forEach(num =>{
    return num / 2
}) // [1,2,3]
let array1 = [10,20,30]
let newArr = []
array1.forEach(num =>{
    newArr.push(num / 10)
})
return newArr // [1,2,3]
Time Complexity - O(n) linear time complexity 

sort()
sorts an array based on alphabetic or numeric or either ascending or descending
ex.
let array = [1, 3, 2, 4]
return array.sort() // [1,2,3,4]
let array1 = ['pears','apples','kiwi','dragonfruit']
return array1.sort() // ['apples','dragonfruit','kiwi','pears']
let array2 = [10,43,23,100,230]
retturn array2.sort() // [10,100,23,230,43]
Time Complexity - O(n log(n)) Logarithmic running time



pop()
it removes the last item in a array and returns the element
ex.
let array = [1,2,3,4]
return array.pop() // 4
let array1 = ['bananas','apples','kiwi']
return array1.pop() // 'kiwi'
return array.pop() // 3
Time Complexity - O(1) constant time complexity 

shift()
removes an element at the beginning of the array
ex.
let array = [1,2,3,4]
return array.shift() // 1
let array1 = ['bananas','apples','kiwi']
return array1.shift() // 'bananas'
return array.shift() // 2
Time Complexity - O(n) linear time complexity 


push()
adds elements to the end of an array
ex.
let array = []
array.push(1)
return array // [1]
array.push('joe')
return array // [1,'joe']
array.push('malon')
return array // [1,'joe','malon']
Time Complexity - O(1) constant time complexity 

unShift()
adds an element to the beginning and returns the length of the array
ex.
let array = [1,2]
return array.unShift(3,4) // 4
return array.unShift(5) // 5
let array1 = ['bananas','apples']
return array.unShift('kiwi') // 3
Time Complexity - O(n) linear time complexity 

includes()
checks to see if an element is present in an array
ex.
let array = [2,4,5,6,7]
return array.includes(3) // false
return array.includes(2) // true
return array.includes(6) // true
Time Complexity - O(n) linear time complexity 


indexOf()
returns the index of a specified element which takes 2 parameters (element, fromIndex)
ex.
let array = [1,2,3,4,5]
return array.indexOf(1) // 0
return array.indexOf(6) // -1
return array.indexOf(3) // 2
Time Complexity - O(n) linear time complexity 


every()
tests all elements that make a provided function true
ex.
let array = [13,54,32,16,19,32,65]
return array.every((element) =>{
    element > 5
}) // true
return array.every((element) =>{
    element > 20
}) // false
let array1 = [19,20,25,50]
return array1.every((element) =>{
    element > 18
}) // true
Time Complexity - O(n) linear time complexity 


charAt()
gives the users the character of a string at a given index
ex.
let charAtArray = 'abcd'
charAtArray.charAt(2) // 'c'
charAtArray.charAt(0) // 'a'
charAtArray.charAt(3) // 'd'
TimeComplexity - O(1) constant time complexity 


charCodeAt()
returns the character code at a given index 
ex.
let string = 'the boat was fast'
string.charCodeAt(5) = 111 //o
string.charCodeAt(7) = 116 //t
string.charCodeAt(2) = 103 //e
Time Complexity - O(1) constant time complexity 


concat()
method that allows 2 arrays to be combined into one new array
ex.
let array1 = ['L','E','O','N']
let array2 = ['N','O','E','L']
return array1.concat(array2) // ['L','E','O','N','N','O','E','L']

let array1 = ['j','o','e']
let array2 = ['m','a','l','o','n']
return array1.concat(array2) // ['j','o','e','m','a','l','o','n']

let array1 = ['1','2','3','4','5']
let array2 = ['6','7','8','9','10']
return array1.concat(array2) // ['1','2','3','4','5','6','7','8','9','10']
Time Complexity - O(n) linear time complexity 

includes()
checks to see if an element is present in an array
ex.
let array = ['Humpty dumpty sat on a wall, Humpty Dumpty had a great fall']
return array.includes('sat') // true
return array.includes('humpty') //false
return array.includes('Humpty') //true
Time Complexity - O(n) linear time complexity 

indexOf()
checks to see the index of a given value in an array
ex.
let array = ['apple','banana','kiwi','pears']
return array.indexOf(2) // 'kiwi'
return array.indexOf(0) // 'apple'
return array.indexOf(3) // 'pears'
Time Complexity - O(n) Linear time complexity 


match() -string method
returns any matching elements based on a given expression
ex.
let string = 'The graphics card market is currently bad'
let text1 = 'a'
return string.match(text1) // ['a','a','a','a']
let text2 = /[A-Z]/g
return string.match(text2) // ['T']
let text3 = /[a-z]/g
return string.match(text3) // ['h','e','g','r','a','p','h','i','c','s','c','a','r','d','m','a','r','k','e','t','i',s','c','u','r','r','e','n','t','l','y','b'a'd']

Time Complexity - O(n) linear time complexity 



repeat()
returns a new string with copies of a string a given amount of times
ex.
let string = 'peanutbutter jelly time '
return `It's${string.repeat(10)}` // 'It's peanutbutter jelly time peanutbutter jelly time peanutbutter jelly time peanutbutter jelly timepeanutbutter jelly time peanutbutter jelly time peanutbutter jelly time peanutbutter jelly time peanutbutter jelly time peanutbutter jelly time '
let word = 21
return word.repeat(21) // 212121212121212121212121212121212121212121
let string = 'hello'
return string.repeat(5) // hellohellohellohellohello
Time Complexity - O(n) linear time complexity 


replace()
replaces a string with a given string
ex.
let string = 'The yellow dog ran across the atlantic ocean'
return string.replace('yellow', 'blue') // The blue dog ran across the atlantic ocean
return string.replace('dog', 'cat') // The blue cat ran across the atlantic ocean
returrn string.replace('atlantic','pacific') // The blue cat ran across the pacific ocean
Time Complexity - O(n) linear time complexity 



search()
searches for a given string and returns the position of the match
ex.
let string = 'The yellow dog ran across the atlantic ocean'
return string.search(yellow) // 4
return string.search(ocean) // 39
return string.search(across) // 19
Time Complexity - O(n) linear time complexity 


slice()
return an element or string based on a given start index and/or end index
ex.
let array = ['a','b','c','d','e']
let string = 'The yellow dog ran across the atlantic ocean'
return array.slice(2,3) // c
return array.slice(3) // ['d','e']
return string.slice(4,10) // yellow
Time Complexity - O(n) linear time complexity 



split()
able to split a string into an array by character , string , sentences
ex.
let string = 'The yellow dog ran across the atlantic ocean'
let string1 = 'yellow'
return string.split(' ') // ['The', 'yellow', 'dog' ,'ran' ,'across', 'the', 'atlantic', 'ocean']
return string1.split('') // ['y','e','l','l','o','w']
let stringChar = string1.split('')
return stringChar[4] // o
Time Complexity - O(n) linear time complexity 


substr()
returns a portion of a string with a given index and/or end
ex.
let string = 'The yellow dog ran across the atlantic ocean'
return string.substr(3,5) // ' ye'
return string.substr(0,2) // 'The'
return string.substr(10,15) // 'don r'
Time Complexity - O(n) linear time complexity 

toLowerCase()
convertes a given string into lowercase letters
ex.
let string = 'HELLO WORLD'
return string.toLowerCase() // 'hello world'
let string1 = 'HeLlOw WoRlD'
return string.toLowerCase() // 'hello world'
let string2 = 'The Yellow Dog Ran Across The Atlantic Ocean'
return string2.toLowerCase() // 'the yellow dog ran across the atlantic ocean'
Time Complexity - O(n) linear time complexity 

toUpperCase()
converts a given string into uppercase letters
ex.
let string = 'hello world'
return string.toLowerCase() // 'HELLO WORLD'
let string1 = 'HeLlOw WoRlD'
return string.toLowerCase() // 'HELLO WORLD'
let string2 = 'The Yellow Dog Ran Across The Atlantic Ocean'
return string2.toLowerCase() // 'THE YELLOW DOG RAN ACROSS THE ATLANTIC OCEAN'
Time Complexity - O(n) linear time complexity 

trim()
removes any whitespace from a given string
ex.
let string = '     Hello World '
return string.trim() // 'Hello World'
let string1 = '   Banana   !                        '
return string1.trim() // 'Banana   !'
let string2 = '   holy   cow!   '
return string2.trim() // 'holy   cow!'
Time Complexity - O(n) linear time complexity 

