## Avgjør hvilken O-notasjon hver algoritme har!

### 1 - n er len(array)

```python
ALGORITHM 1
INPUT: An array of size >= 3 containing integers.
OUTPUT: Sum of first 3 integers.


PROC sum_three_elements(array):
    return array[0] + array[1] + array[2]
```

### 2 - n er len(input_string)

```python
PROC string_contains_space(input_string):
    for char in input do:
        if char equals ' ' then:
            return True
    return False
```

### 3 - n er n

```python
PROC print_number_many_times(n):
    for i <- to n do:
        print n
```

### 4 - n er |array| (lengden av array)

```python
PROC contains_duplicate(array):
    for i <- 0 to |array| do:
        for j <- 0 to |array| do:
            if i != j and array[i] equals array[j] then:
                return True
    return False

```

### 5 - n er |array| (lengden av array)

```python
PROC contains_duplicate_smarter(array):
    for i <- 0 to |array| do:
        for j <- i+1 to |array| do:
            if array[i] == array[j] then:
                return True
    return False
```

### 6 - n er n

```python
PROC multiply_by_two(n):
    current <- 1
    while current <= n do:
        print current
        current <- current * 2
```

### 7 - n er |array1|, m er |array2|

```python
PROC sums_multiplied(array1, array2):
    sum1 <- 0
    sum2 <- 0

    for element in array1 do:
        sum1 <- sum1 + element

    for element in array2 do:
        sum2 <- sum2 + element

    return sum1*sum2
```

### 8 - n er |array1|, m er |array2|, k er k

```python
PROC sums_multiplied_k_times(array1, array2, k):
    sum <- 0
    for ctr in range(k) do:
        sum <- sum + sums_multiplied(array1, array2)

```
