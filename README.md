# IT313 TypeScript Foundations

## Problem

This project converts the Enrollment Eligibility Checker from JavaScript to TypeScript. It calculates each student's average grade and determines whether they are **Passing** or **Probation**. It also generates remarks for probation students and calculates the class average and number of passing students.

## TypeScript Concepts Applied

- **Interfaces** – Define the structure of `Enrollee` and `EligibilityReport`.
- **Enum** – Ensures student status is only `Passing` or `Probation`.
- **Union Type** – Allows the batch ID to be either a `string` or `number`.
- **Optional Property** – `remarks` is only included for probation students.
- **Generics** – The `groupBy<T>()` function groups reports by status while keeping type safety.
- **Async/Await & Promise** – Simulates retrieving enrollee data from a registrar API.
- **map() and reduce()** – Used to create reports and calculate the class average.
- **Strict TypeScript** – `"strict": true` is enabled to catch type errors before running the program.

## How to Run

Install the required tools:

```bash
npm install
```

Run the TypeScript files using `ts-node`:

```bash
npx ts-node gradeUtils.ts
npx ts-node main.ts
```

Check for TypeScript errors without running the program:

```bash
npx tsc --noEmit
```

