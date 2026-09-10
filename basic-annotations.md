## Basic commands 
``go run:`` Run a .go file

``go mod init:`` Initialize a new module on a package. The module manage the dependeces inside GO just like the package.json on NodeJS.

``go build:`` After the go module was created you can run the ``go build`` for compile all go files in the same page or other to a binary file. 

For run this file you need to write in terminal the name of file with ``¨./¨`` eg(¨./modules¨)

``go get <url> :`` Use for install a external package and update the go.mod file 
``go mod tidy:`` Remove all diuse packages on go.mod file
## Basic snippet of code

main.go

```
package main

import ¨fmt¨

func Main () {
    fmt.Println(¨Hello World¨)
}
```

Importing a external package
```
package main
import (
    ¨fmt¨,
    ¨github.com/test¨
)
```

## Naming a function

If a functions starts with a the first letter being an upercase letter it will be visible for all packages. Otherwise it will visible only within the package where it was written.

```
-----#Module
----#main.go
----#Write_Package
---#write.Go

func Write() // Will be visible for all packages
func write() // Only for the Write_Package
```

A good pratice if you will export a function is add a comment right on top of the function.
```
// this function write a hello world
func HelloWorld(){
    fmt.Println(¨Hello World¨)
}
```
## Variable declaration

We can declare a variable with two ways:

Using var and the type or variable 
```
var myFirstString string
```

Or using the := the value will be add defining the value of the variable
```
mySecondString := "Texting something in this block of code."
```