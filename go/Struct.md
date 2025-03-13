# Struct

Struct == Object

### Creating a struct (basically it is creating a new data type)

```go
type User struct{
	firstName string
	lastName string
	dof string
	created time.Time
}
//func belongs to specific struct
func (user *User) outputDetails(){
	fmt.Printf("My name is %v %v (born on %v)",user.firstName,user.lastName, user.dof)
}
func main(){
	//creating
	var newUser User
	...
	//defining
	newUser = User(firstName: {value},lastName: {value}, ....)
}
```