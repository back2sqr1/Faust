---
media_link: https://www.youtube.com/watch?v=FgnxcUQ5vho&t=4
---
#Video

Jest: 

Example: Clone Array (array)  - > return [...array]

# Start

```bash
npm init -y
npm i --save-dev jest
```
Only use in development (save dev)

Look in package.json
Go to scripts:
test: "jest"

## Creating my first test

Create file : file_name.test.js (or ts)

```typescript
import { sum } from 'file location'

// creates function
// description is shown in console
test('description', () => {
	expect(sum(1, 2)).toBe(3) // we expect something
});

.toBe -> (reference equal)
.toEqual -> (value equal)
.not.toBe()-> not reference equal
```
Lambda Function is called when the npm test is run
### Coverage

```json
"test": "jest --coverage" 
```

Tells us which functions are tested

## Why test

Tests can investigate changes and make sure everything passes


