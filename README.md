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









