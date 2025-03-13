# Maps

Maps == List with named index (it is key value pair)\

 //use to label data

`websites := map[string]string{ "Google":"www.google.com"}`

    `data type:    key   value`

```go
websites := map[string]string{ "Google":"www.google.com"}
//data-type-for: key    value
fmt.Println(websites["Google"])
delete(websites,"Google")
```