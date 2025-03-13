# Lists

List ==  Array

```go
//1
var fruits [3]string
//2
// {*var_name*} := [*no of elements*]*data_type*{*elements*}
fruits := [3]string{"apple","mango","banana"}
```

### Slices

```go
fruits := [3]string{"apple","mango","banana"}
first_two_elements := fruits[0:2]
```

**[a:b] → index from a to b including a and excluding b**

**[:b] → index from 0 to b including 0 and excluding b**

**[a:] → index from a to *last-index* including a and *last-index***

---

Slices are pointer changing value in slices changes value in acutal list.

```go
	my_fav := fruits[:3]
	most_fav := my_fav[1]
	my_fav[1] = "lemon"
//this will change actual list: fruits
```

**len() → no of elements in list**

**cap() → total no elements in underlying array (array from whic slice is originated)**

## Dynamic Lists

**`append(list,element) → returns a list with given element at rightmost of given list`**

```go
fruits := []strings{"apple","mango","banana"}
//re-defining fruits with new element
fruits = append(fruits,"lemon")
//multiple elements can be added
fruits = append(fruits,"strawberry","kiwi","orange")
```

**To add a list in a list:**

```go
list1 := []int{1,2,3}
list2 := []int{4,5,6}
//appending list2 in list1
list1 = append(list1, list2...)
// *list2...* will change list2 's elements in individual 
//elements seperated by comma
```