# If you're interested in this field and want to simplify your life

In just 2-3 weeks, you can learn to write scripts if you dedicate 6-8 full hours per week.  

    The more time you invest, the better the results.

## A few tips:

- Look at the code as a list of tasks; each function solves a specific problem.  
- Functions are organized into classes, which can be used as references in other parts of the code.  
- Use the cursor; I recommend subscribing.

## I program in TypeScript  
because it is more organized and easier to work with.  
I use architectural approaches like Object Oriented Programming and micro-services.  
Each script has a chronological structure: imports, data types, functions, exports;

### More details:

- **Imports** – References to functions in other files. Also known as dependencies. They can be written by the developer or imported from downloaded packages (libraries). For example, Python uses pip, NodeJS uses npm.  
- **Data Types** – numbers, strings, interfaces, types, enums, booleans, arrays, etc. Mostly these are basic data types, such as numbers, strings, arrays, etc.  
- **Functions** – Basically gateways. They take something in and produce something out. They should be simple and clear. Function names usually hint at the task they solve.  
- **Exports** – What we want to make available for other files.

#### Sidenote:
Data “logistics” is key in proper programming.  
We load data from somewhere and deliver it somewhere else—to other functions, output them in the terminal, transmit them via API, etc.

Example syntax:  
"//" <— These are comments in TS/JS. They’re for the developer.

```typescript
// 1. Import functions from other files.
import { greeting } from './greeting.ts';

// 2. Define variables:
const x = 1;
const y = 2;
const z = 3;

// 2. Rename the imported function:
const Hello = greeting;

// 3. Output the result to the terminal.
console.log(Hello);

// 4. Create an interface for the variables:
interface CalculationResults {
    result1: number;
    result2: number;
    result3: number;
}

// 5. Declare a function that takes 3 arguments and returns a number.
// The body of the function is defined within the {} brackets:

console.log(`📨 Data received, starting calculations`);
function calculationResult(x: number, y: number, z: number) {
    
    console.log(`🧮 Calculating result 1`);
    const calculationResult1 = (x + y) * z;

    console.log(`🧮 Calculating result 2`);
    const calculationResult2 = (x + z) * y;

    console.log(`🧮 Calculating result 3`);
    const calculationResult3 = (x + y) * z;

    console.log(`🎁 Packing data into an object`);
    const calculationResults = {
        calculationResult1,
        calculationResult2,
        calculationResult3
    };

    console.log(`🙌 Returning results`);
    return calculationResults;
}

// 6. Call the function and output the result to the terminal.
const result = calculationResult(x, y, z);
console.log(`👉 Your result: `, result);

// 7. Export the object so it’s available in other files.
export { calculationResult };
```

Expected result:

```
📨 Data received, starting calculations
🎁 Calculating result 1
🎁 Calculating result 2
🎁 Calculating result 3
🎁 Packing data into an object
🙌 Returning results
👉 Your result:  { calculationResult1: 6, calculationResult2: 9, calculationResult3: 12 }
```

## If you can solve this task, then you're ready to write basic scripts:  
Time allocated: 30-60 minutes maximum. If you can't, then you've missed something and need to review the material or clarify the details.
It's a task, so you will have to resolve few steps by yourself. 

1. Create a project on NodeJS (npm init -y)
2. Create an index.ts file
3. Create a hello.ts file
4. Import the greeting function in index.ts
5. Copy the code from the example above into index.ts
6. Run index.ts

Errors are stepping stones to understanding what you're doing wrong and correcting yourself in time. More errors mean more experience.

Chapter 2 will cover more complex concepts and practices that help you make more powerful scripts, process larger data objects, and make sure that you will be able to write clean code that works for you.


