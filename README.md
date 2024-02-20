# Extra_Knowlage
Janke kya krna he aap ko


**Event Emitter**

Create Coustum events and handle coustum events Models
two types - on(function) and emit

///
const EventEmitter = require('events');  /// import

// Importing events 
const EventEmitter = require('events'); 

// Initializing event emitter instances  
var eventEmitter = new EventEmitter(); 
  
// Registering to myEvent  
eventEmitter.on('myEvent', (msg) => { 
   console.log(msg); 
}); 
  
// Triggering myEvent 
eventEmitter.emit('myEvent', "First event"); 

//Output:
First event


**stack trace** 
console.log(Error().stack);
Error
    at file:///E:/Yanish/2024/2024-Socket.IO/Freee.js:1:13
    at ModuleJob.run (node:internal/modules/esm/module_job:218:25)
    at async ModuleLoader.import (node:internal/modules/esm/loader:329:24)
    at async loadESM (node:internal/process/esm_loader:28:7)
    at async handleMainPromise (node:internal/modules/run_main:113:12)
    
**Call Stack in JavaScript**
js Engine keep track of function call in program
 Last In,First Out (LIFO) data structure
call Stack Image URL - https://media.geeksforgeeks.org/wp-content/uploads/20201213103357/global.png

**NPM AND NPX**
npm - node packeg mangaer 
npx - node packege executer

**Async/Await**
Async/Await is a special syntax to work with promises in a more comfortable fashion. It’s easy to understand and use. Adding the keyword async before a function ensures that the function returns a promise and the keyword await makes JavaScript wait until that promise settles and returns the result.

**git Switch -c <branchname>**
tranfer commite one branch to another branch 

**process.nextTick() setImmediate() setTimeout()**
A function passed to process.nextTick() is always call event loop end after start new event loop befor they call first allways after event lopp execute

**This means it will always execute before setTimeout and setImmediate**.

A **process.nextTick**  callback is added to     **process.nextTick queue**.
A **Promise.then()**   callback is added to promises     **microtask queue**.

A **setTimeout**, **setImmediate**     callback is added to     **macrotask queue**        **setTimeout** - Timer Queue      **setImmediate** - check handeler/ queue.

**Path Module**
import path from "path";  //// import path mode here 

console.log(path.dirname("E:/Yanish/2024/2024-Socket.IO"));
console.log(path.extname("E:/Yanish/2024/2024-Socket.IO"));
console.log(path.basename("E:/Yanish/2024/2024-Socket.IO"));
console.log(path.parse("E:/Yanish/2024/2024-Socket.IO"));

///**Out Put**
E:/Yanish/2024 
.IO
2024-Socket.IO
{
  root: 'E:/',
  dir: 'E:/Yanish/2024',
  base: '2024-Socket.IO',
  ext: '.IO',
  name: '2024-Socket'
}

**fs Module**
file System 

**Forget PassWord**

function generatePassword(length) {
  var chars = "0123456789abcdefghijklmnopqrstuvwxyz#$%^&@";
  var result = "";
  for (var i = length; i > 0; --i)
    result += chars[Math.floor(Math.random() * chars.length)];
  return result;
}






