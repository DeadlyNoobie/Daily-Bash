# Day 1

### [Problem Statement](https://www.codewars.com/kata/514b92a657cdc65150000006/train/shell)

**With above problem statement**

**we first take input as first argument**

**we loop i and check if the number is divisible by 3 or 5 if so we add that number to the sum var and at last we print that sum var**


```
#!/bin/bash

n=$1
sum=0
for ((i=0; i<$n; i++)); do
  if [ $((i%3)) -eq 0 ] || [ $((i%5)) -eq 0 ]; then
    sum=$((sum+i));
  fi
done

echo $sum
```
