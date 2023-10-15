# First hackerrank Plus Minus

Variables are declared as <mark> var</mark> while constant are declared as  <mark> let </mark>

``` swift
// Example of declare empty array 
var arr: [Int] = []

func plusMinus(arr: [Int]) -> Void {

    var positive : Double = 0
    var negative : Double = 0
    var neutral  : Double = 0
    var size = Double(arr.count)
    // for loop example
    for i in arr {
        if i > 0 {
          positive += 1  
        } 
        else if i<0{
            negative += 1
        }
        else if i == 0
        {
            neutral += 1
        }
    } 
    
    positive = positive/size
    negative = negative/size
    neutral = neutral/size
    
    print(positive)
    print(negative) 
    print(neutral) 
}
```

Example of plus minus using Indexes

``` swift
func plusMinus(arr: [Int]) -> Void {
    var positive : Double = 0
    var negative : Double = 0
    var neutral  : Double = 0
    var size = Double(arr.count)
    let s = arr.count
    for i in 0..<s {
        if arr[i] > 0 {
          positive += 1  
        } else if arr[i]<0{
            negative += 1
        }
        else if arr[i] == 0
        {
            neutral += 1
        }
    } 
    
    positive = positive/size
    negative = negative/size
    neutral = neutral/size
    
    print(positive)
    print(negative) 
    print(neutral) 
}
```