### The Monkey Programming Language

```
let age = 1;
let name = "Monkey";
let result = 10 * (20 / 2);

let myArray = [1, 2, 3, 4, 5];

let monkey = {"name": "Monkey", "age": 10};

myArray[0]      // => 1 
monkey["name"]  // => "Monkey"

let add = fn(a, b) { return a + b; };

add(1, 2);

let fibonacci = fn(x) {
    if (x == 0) {
        0
    } else {
        if (x == 1) {
            1
        } else {
            fibonacci(x - 1) + fibonacci(x - 2);
        } 
    }
};

let twice = fn(f, x) { 
    return f(f(x));
};

let addTwo = fn(x) { 
    return x + 2;
};

twice(addTwo, 2); // => 6

```

To run REPL checkout and execte `go run main.go`