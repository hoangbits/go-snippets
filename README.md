# go-snippets
 

### Table of Contents
| No. | Questions |
|---- | ---------
|1  | [How to generate a random bool](#How-to-generate-random-bool)|
|2  | 
|3  | 
|4  | 
|5  | 
|6  | 
|7  | 
|8  | 
|9  | 
|10 | 
|11 | 
|12 | 
|13 | 
|14 | 
|15 | 
|16 | 
|17 | 
|18 | 
|19 | 
|20 | 
|21 | 
|22 | 
|23 | 
|24 | 
|25 | 
|26 | 
|27 | 
|28 | 
|29 | 
|30 | 




**[⬆ Back to Top](#table-of-contents)**
### How to generate a random bool
```go
// RandBool This function returns a random boolean value based on the current time
func RandBool() bool {
	rand.Seed(time.Now().UnixNano())
	if rand.Intn(2) == 1 {
		return true
	}
	return false
}