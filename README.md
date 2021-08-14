# oopJS
Bind VS Apply VS Call

**Call( ):** 

    The call() method invokes a function with a given 'this' value and arguments provided one by one. This means that we can call any function, and explicitly specify what 'this' should reference within the calling function.


var name1 ={ firstName:'Yuvi',lastName:'Raj'};
var name2 = { firstName:'first', lastName:'last'};

function print(arg1,arg2){
  console.log(arg1+' '+this.firstName+' '+this.lastName+' '+arg2)

}

print.call(name1,'Hi','...'); 


**Apply( )**

   Invokes the function and allows you to pass in arguments as an array.
   
var name1 ={ firstName:'Yuvi',lastName:'Raj'};
var name2 = { firstName:'first', lastName:'last'};

function print(arg1,arg2){
  console.log(arg1+' '+this.firstName+' '+this.lastName+' '+arg2)

}
   
   print.apply(name1,['Hi','...']);
   
   
**Bind()**

   Returns a new function, allowing you to pass in an array and any number of arguments.
   
   
var name1 ={ firstName:'Yuvi',lastName:'Raj'};
var name2 = { firstName:'first', lastName:'last'};

function print(arg1,arg2){
  console.log(arg1+' '+this.firstName+' '+this.lastName+' '+arg2)

}
   
  var printname1= print.bind(name1,['Hi','...']);
  
  printname1('hello','fine');


   
   







