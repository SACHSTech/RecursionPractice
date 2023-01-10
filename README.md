# Recursion Practice


### Problem Set 1

#### count7 
`public static int count7(int n)`  
Given a non-negative int n, return the count of the occurrences of 7 as a digit, so for example 717 yields 2. (no loops). Note that mod (%) by 10 yields the rightmost digit (126 % 10 is 6), while divide (/) by 10 removes the rightmost digit (126 / 10 is 12).
```
count7(717) → 2
count7(7) → 1
count7(123) → 0
```


#### countHi
`public static int countHi(String str)`  
Given a string, compute recursively (no loops) the number of times lowercase "hi" appears in the string.
```
countHi("xxhixx") → 1
countHi("xhixhix") → 2
countHi("hi") → 1
```

### Problem Set 2

#### changePi
`public static String changePi(String str) `  
Given a string, compute recursively (no loops) a new string where all appearances of "pi" have been replaced by "3.14".
```
changePi("xpix") → "x3.14x"
changePi("pipi") → "3.143.14"
changePi("pip") → "3.14p"
```
#### pairStar
`public static String pairStar(String str)`  
Given a string, compute recursively a new string where identical chars that are adjacent in the original string are separated from each other by a "*".
```
pairStar("hello") → "hel*lo"
pairStar("xxyy") → "x*xy*y"
pairStar("aaaa") → "a*a*a*a"
```


### Problem Set 3

#### array220
`public static boolean array220(int[] intNums, int index)`  
Given an array of ints, compute recursively if the array contains somewhere a value followed in the array by that value times 10. We'll use the convention of considering only the part of the array that begins at the given index. In this way, a recursive call can pass index+1 to move down the array. The initial call will pass in index as 0.
```
array220([1, 2, 20], 0) → true
array220([3, 30], 0) → true
array220([3], 0) → false
```

#### stringClean
`public static String stringClean(String str)`  
Given a string, return recursively a "cleaned" string where adjacent chars that are the same have been reduced to a single char. So "yyzzza" yields "yza".
```
stringClean("yyzzza") → "yza"
stringClean("abbbcdd") → "abcd"
stringClean("Hello") → "Helo"
```

#### strCopies
`public static boolean strCopies(String str, String sub, int n)`  
Given a string and a non-empty substring sub, compute recursively if at least n copies of sub appear in the string somewhere, possibly with overlapping. N will be non-negative.
```
strCopies("catcowcat", "cat", 2) → true
strCopies("catcowcat", "cow", 2) → false
strCopies("catcowcat", "cow", 1) → true
```
