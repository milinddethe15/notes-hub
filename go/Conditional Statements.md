# Conditional Statements

## `If` statements:

```go
if age >= 18 {
	fmt.Println("Welcome to club")
} else if age>15 {
	fmt.Println("Welcome to club, but you can't drink Alcohol")
} else {
	fmt.Println("Goodbye!")
}
```

if statements works on boolen value of the conditons.

`&& → and`

`|| → or`

`!= → not equal`

---

---

## Loops

repeat some steps 

Sum till n number:

```go
sum := 0
for i := 1; i <= n; i++{
	//code to repeat	
	sum = sum + i
}
```

Factorial of n:

```go
factorial := 1
for i := 1; i <= n; i++{
	//code to repeat	
	factorial = factorial * i
}
```

GO doesnt have `while` it has modified version of `for`. (infinite loop)

`for {*condition*} {
some to repect infinity until condition is made false`

`}`

---

## Looping in map, list, slices

```go
for index,value := range data{
	//iterate every values of data types
}
```

## Continue and Break

Continue → break single iteration (skips a single loop) 

Break → break whole iterations (skips the looping)