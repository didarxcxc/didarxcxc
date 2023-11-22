// 1
// function fullName() {
//     console.log("Didar");
// }
// 2
// function fullName(firstName, lastName) {
//     return `${firstName} ${lastName}`;
// }
// console.log(fullName("Di", "dar"));
// 3
// function addNumbers(num1, num2) {
//     return num1 + num2;
// }
// let result = addNumbers(9, 11);
// console.log(result);
// 4
// function areaOfRectangle(length, width) {
//     return length * width;
// }
// let result = areaOfRectangle(7, 7);
// console.log(result);
// 5
// function perimeterOfRectangle(length, width) {
//     return 2 * (length + width);
// }
// let result = perimeterOfRectangle(8, 2);
// console.log(result);
// 6
// function volumeOfRectangularPrism(length, width, height) {
//     return length * width * height;
// }
// let result = volumeOfRectangularPrism(5, 9, 4);
// console.log(result);
// 7
// function areaOfCircle(radius) {
//     return Math.PI * radius ** 2;
// }
// let result = areaOfCircle(19);
// console.log(result);
// 8
// function circumOfCircle(radius) {
//     return 2 * Math.PI * radius;
// }
// let result = circumOfCircle(20);
// console.log(result);
// 9
// function calculateDensity(mass, volume) {
//     return mass / volume;
// }
// let result = calculateDensity(250, 89);
// console.log(result);
// 10
// function calculateSpeed(distance, time) {
//     return distance / time;
// }
// let result = calculateSpeed(100, 2);
// console.log(result);
// 11
// function calculateWeight(mass, gravity) {
//     return mass * gravity;
// }
// let result = calculateWeight(25, 5.5);
// console.log(result);
// 12
// function convertCelsiusToFahrenheit(celsius) {
//     return (celsius * 9/5) + 32;
// }
// let result = convertCelsiusToFahrenheit(25);
// console.log(result);
// 13
// function calculateBMI(weight, height) {
//     let bmi = weight / (height ** 2);
//     return bmi;
// }

// function classifyBMI(bmi) {
//     if (bmi < 18.5) {
//         return "Underweight";
//     } else if (18.5 <= bmi && bmi <= 24.9) {
//         return "Normal weight";
//     } else if (25 <= bmi && bmi <= 29.9) {
//         return "Overweight";
//     } else {
//         return "Obese";
//     }
// }
// let bmiResult = calculateBMI(70, 1.75);
// let classification = classifyBMI(bmiResult);
// console.log(`BMI: ${bmiResult}, Classification: ${classification}`);
// 14
// function checkSeason(month) {
//     if (month >= 3 && month <= 5) {
//         return "Spring";
//     } else if (month >= 6 && month <= 8) {
//         return "Summer";
//     } else if (month >= 9 && month <= 11) {
//         return "Autumn";
//     } else {
//         return "Winter";
//     }
// }
// let result = checkSeason(7);
// console.log(result);
// 15
// function findMax(a, b, c) {
//     if (a >= b && a >= c) {
//         return a;
//     } else if (b >= a && b >= c) {
//         return b;
//     } else {
//         return c;
//     }
// }
// console.log(findMax(0, 10, 5));  
// console.log(findMax(0, -10, -2));
// 16
// function solveForX(a, b, c, y) {
//     let x = (-c - b * y) / a;
//     return x;
// }
// let result = solveForX(2, 3, 4, 5);
// console.log(result);
// 17
// function solveQuadratic(a = 0, b = 0, c = 0) {
//     const discriminant = Math.sqrt(b**2 - 4*a*c);
//     const root1 = (-b + discriminant) / (2*a);
//     const root2 = (-b - discriminant) / (2*a);

//     return [root1, root2];
// }
// let result = solveQuadratic(1, 4, 4);
// console.log(result);
// 18
// function printArray(arr) {
//     arr.forEach(value => {
//         console.log(value);
//     });
// }
// let arr = [1, 2, 3, 4, 5];
// printArray(arr);
// 19
// function showDateTime() {
//     const currentDate = new Date();
//     const day = currentDate.getDate().toString().padStart(2, '0');
//     const month = (currentDate.getMonth() + 1).toString().padStart(2, '0');
//     const year = currentDate.getFullYear();
//     const hours = currentDate.getHours().toString().padStart(2, '0');
//     const minutes = currentDate.getMinutes().toString().padStart(2, '0');
//     console.log(`${month}/${day}/${year} ${hours}:${minutes}`);
// }
// showDateTime();
// 20
// function swapValues(x, y) {
//     return [y, x];
// }
// let result = swapValues(3, 4);
// console.log(`x => ${result[0]}, y => ${result[1]}`);
// 21
// function reverseArray(arr) {
//     let reversedArray = [];
//     for (let i = arr.length - 1; i >= 0; i--) {
//         reversedArray.push(arr[i]);
//     }
//     return reversedArray;
// }
// let result = reverseArray(['A', 'B', 'C']);
// console.log(result);
// 22
// function capitalizeArray(arr) {
//     return arr.map(item => item.charAt(0).toUpperCase() + item.slice(1));
// }
// let result = capitalizeArray(['apple', 'banana', 'cherry']);
// console.log(result);
// 23
// function addItem(item, myArray) {
//     myArray.push(item);
//     return myArray;
// }
// let myList = ['apple', 'banana', 'cherry'];
// let result = addItem('orange', myList);
// console.log(result);
// 24
// function removeItem(index, myArray) {
//     if (index >= 0 && index < myArray.length) {
//         myArray.splice(index, 1);
//     }
//     return myArray;
// }
// let myList = ['apple', 'banana', 'cherry'];
// let result = removeItem(1, myList);
// console.log(result);
// 25
// function sumOfNumbers(number) {
//     return Array.from({ length: number }, (_, i) => i + 1).reduce((sum, num) => sum + num, 0);
// }
// let result = sumOfNumbers(5);
// console.log(result);
// 26
// function sumOfOdds(number) {
//     return Array.from({ length: number }, (_, i) => i + 1)
//         .filter(num => num % 2 !== 0)
//         .reduce((sum, oddNum) => sum + oddNum, 0);
// }
// let result = sumOfOdds(7);
// console.log(result);
// 27
// function sumOfEven(number) {
//     return Array.from({ length: number }, (_, i) => i + 1)
//         .filter(num => num % 2 === 0)
//         .reduce((sum, evenNum) => sum + evenNum, 0);
// }
// let result = sumOfEven(8);
// console.log(result);
// 28
// function evensAndOdds(number) {
//     const evens = Array.from({ length: number }, (_, i) => i + 1)
//         .filter(num => num % 2 === 0)
//         .length;

//     const odds = Array.from({ length: number }, (_, i) => i + 1)
//         .filter(num => num % 2 !== 0)
//         .length;

//     console.log(`The number of odds are ${odds}.`);
//     console.log(`The number of evens are ${evens}.`);
// }
// evensAndOdds(100);
// 30
// function generateRandomUserIp() {
//     const ip = Array.from({ length: 4 }, () => Math.floor(Math.random() * 256)).join('.');
//     return ip;
// }
// let result = generateRandomUserIp();
// console.log(result);
// 31
// function generateRandomMacAddress() {
//     const manufacturerIdentifier = [0x00, 0x16, 0x3e];
//     const randomBytes = Array.from({ length: 3 }, () => Math.floor(Math.random() * 256));

//     const mac = [...manufacturerIdentifier, ...randomBytes];
//     const macAddress = mac.map(byte => byte.toString(16).padStart(2, '0')).join(':');
    
//     return macAddress;
// }
// let result = generateRandomMacAddress();
// console.log(result);
// 32
// function randomHexaNumberGenerator() {
//     const randomHex = '#' + Math.floor(Math.random()*16777215).toString(16);
//     return randomHex;
// }
// console.log(randomHexaNumberGenerator());
// 33
// function arrayOfHexaColors(numColors) {
//     const colors = [];
//     for (let i = 0; i < numColors; i++) {
//         const randomHex = '#' + Math.floor(Math.random() * 16777215).toString(16);
//         colors.push(randomHex);
//     }
//     return colors;
// }
// console.log(arrayOfHexaColors(5));
// 34
// function arrayOfRgbColors(numColors) {
//     const colors = [];
//     for (let i = 0; i < numColors; i++) {
//         const randomRgb = `rgb(${Math.floor(Math.random() * 256)}, ${Math.floor(Math.random() * 256)}, ${Math.floor(Math.random() * 256)})`;
//         colors.push(randomRgb);
//     }
//     return colors;
// }
// console.log(arrayOfRgbColors(5));
// 35
// function convertHexaToRgb(hexColor) {
//     hexColor = hexColor.replace('#', '');
//     const r = parseInt(hexColor.substring(0, 2), 16);
//     const g = parseInt(hexColor.substring(2, 4), 16);
//     const b = parseInt(hexColor.substring(4, 6), 16);
//     return `rgb(${r}, ${g}, ${b})`;
// }
// console.log(convertHexaToRgb('#1a2b3c'));
// function convertRgbToHexa(rgbColor) {
//     const rgbValues = rgbColor.match(/\d+/g);
//     const hexColor = rgbValues.map(value => {
//         const hex = parseInt(value).toString(16);
//         return hex.length === 1 ? '0' + hex : hex;
//     });
//     return `#${hexColor.join('')}`;
// }
// console.log(convertRgbToHexa('rgb(26, 43, 60)'));
