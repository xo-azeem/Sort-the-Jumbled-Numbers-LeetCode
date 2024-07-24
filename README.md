# Sort the Jumbled Numbers

LeetCode Q # 2191.

You are given a 0-indexed integer array mapping which represents the mapping rule of a shuffled decimal system. mapping[i] = j means digit i should be mapped to digit j in this system.

The mapped value of an integer is the new integer obtained by replacing each occurrence of digit i in the integer with mapping[i] for all 0 <= i <= 9.

You are also given another integer array nums. Return the array nums sorted in non-decreasing order based on the mapped values of its elements.

Notes:

- Elements with the same mapped values should appear in the same relative order as in the input.</br>
- The elements of nums should only be sorted based on their mapped values and not be replaced by them.
 
Example 1:

> Input: mapping = [8,9,4,0,2,1,3,5,7,6], nums = [991,338,38]</br>
> Output: [338,38,991]</br>
> Explanation: </br>
> Map the number 991 as follows:</br>
> 1. mapping[9] = 6, so all occurrences of the digit 9 will become 6.</br>
> 2. mapping[1] = 9, so all occurrences of the digit 1 will become 9.</br>
> Therefore, the mapped value of 991 is 669.</br>
> 338 maps to 007, or 7 after removing the leading zeros.</br>
> 38 maps to 07, which is also 7 after removing leading zeros.</br>
> Since 338 and 38 share the same mapped value, they should remain in the same relative order, so 338 comes before 38.</br>
> Thus, the sorted array is [338,38,991].</br>

Example 2:

> Input: mapping = [0,1,2,3,4,5,6,7,8,9], nums = [789,456,123]</br>
> Output: [123,456,789]</br>
> Explanation: 789 maps to 789, 456 maps to 456, and 123 maps to 123. Thus, the sorted array is [123,456,789].</br>

My Solution Analysis:

<div align = "center">

  ![image](https://github.com/user-attachments/assets/d815bd30-a6ff-4c85-b7d6-4e9aa0a05805)

  Time complexity: O(n ∗ log(n)).</br>Space complexity: O(n).
</div>
