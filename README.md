# Coderetrat JS Tutorial

### Install Node.js
Follow the link https://nodejs.org/en/ and download "LTS" version

### Install NPM and Mocha
Now initialize npm. We will use it to create a `package.json` with the Mocha framework:
    
    npm init
When asked for the details of the application provide the following:
* name: hello-world
* entry point: app.js
* test command: mocha

You can use any framework for testing.

You can confirm the rest of the values with enter.

Now install Mocha framework (again, you can use any library for testing purposes):

    npm install mocha
    
### Getting started

Create `test.js` file and put your code in there.

> Example:
>
>     var assert = require('assert');
>     describe('Array', function() {
>       describe('#indexOf()', function() {
>         it('should return -1 when the value is not present', function() {
>           assert(equal([1, 2, 3].indexOf(4), -1);
>         });
>      });
>     });

Set up a test script in `package.json`:

    "scripts": {
      "test": "mocha"
    }
Then run tests with:
     
    npm test
