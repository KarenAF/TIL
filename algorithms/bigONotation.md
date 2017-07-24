7/23/17 Big O Notation

Evaluating the efficiency of one possible solution to the following coding problem: Write a method that accepts an array and returns true if the array contains any duplicate values, and false if it does not.

(Inefficient) Solution with efficiency of O(n²):

```
def findDuplicates(array)
  array.each do |original_value|
    times_repeated = 0
    array.each do |compared_value|
      if original_value == compared_value
        times_repeated += 1
      end
    end
    if times_repeated > 1
      puts original_value
      return true
    else
      return false  
    end  
  end  
end

array = [1, 4, 2, 3, 4, 5, 2, 2]    
puts findDuplicates(array)    
```
This solution is inefficient because each value in the array is compared to each other value, so each value is compared n times. So for each increase in the number of values, that's n more actions the computer must take. Thus, the efficiency is n * n.