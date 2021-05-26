veify input belong to number or not

* "123" -> true

* 123 -> true

* undefined -> false

* null -> false 

* "12a3" -> false

* "" -> false


# Example 

    var { isNumber, isEven, isOdd } = require("./index");

    isNumber(10); //-> true
    isNumber("10");  -> true 
    isNumber(""); -> false 
    isNumber(undefined); -> false
    isNumber(null);  -> false
    isNumber("abc");  -> false

    isEven(10);  -> true
    isEven(9);  -> false
    isEven("a12");  ->  throw "Input parameter is not a number!";
    isEven(undefined); ->  throw "Input parameter is not a number!";
    isEven(null);  ->  throw "Input parameter is not a number!";

    isOdd(10);  -> false
    isOdd(9);  -> true
    isOdd("abc");  ->  throw "Input parameter is not a number!";
    isOdd(undefined); ->  throw "Input parameter is not a number!";
    isOdd(null);  ->  throw "Input parameter is not a number!";

