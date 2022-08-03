# What-i-learned-8-3-22

// what i learn using testing

{
  "name": "learn",
  "version": "1.0.0",
  "description": "> ### **Tips: Before you Begin** > #### **To view your code and instructions side-by-side**, select the following in your VSCode toolbar: > - View -> Editor Layout -> Two Columns > - To view this file in Preview mode, right click on this README.md file and `Open Preview` > - Select your code file in the code tree, which will open it up in a new VSCode tab. > - Drag your assessment code files over to the second column.  > - Great work! You can now see instructions and code at the same time.  > - Questions about using VSCode? Please see our support resources here:   > [Visual Studio Code on Coursera](https://www.coursera.org/learn/programming-with-javascript/supplement/roMvE/visual-studio-code-on-coursera) > #### **To run your JavaScript code** > - Select your JavaScript file > - Select the \"Run Code\" button in the upper right hand toolbar of VSCode.   > Ex: It looks like a triangular \"Play\" button.  <br><br>",
  "main": "index.js",
  "scripts": {
    "test": "jest"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "dependencies": {
    "jest": "^28.1.3"
  }
}

// basic function for testing


function timesTwo(num) {
    return num*2
}

module.exports = timesTwo


// tesing the function

const timesTwo = require('./timesTwo');


test('returns the number times 2', () => {
    expect(timesTwo(10)).toBe(20)
});


//it worked and was passed
