Given an array of positive integers arr[], return the second largest element from the array. If the second largest element doesn't exist then return -1.

Note: The second largest element should not be equal to the largest element.

Examples:

Input: arr[] = [12, 35, 1, 10, 34, 1]
Output: 34
Explanation: The largest element of the array is 35 and the second largest element is 34.

### Approach:

1. Initialize Variables: 
   - largest = -1: To store the second highest in the array.
   - secondLargest = -1: To store the second highest value.
2. Traverse the array:
   -Use a for-each loop to go through each number in the array.
3. Comapre each number:
   -If the current number is greater than the largest:
   -Set 'secondLargest = largest'
   -Set 'largest = current number'
   -Else if the number is between 'secondLargest' and 'largest':
   -Update 'secondLargest = current number'
4. Return the second largest number:
   -At the end of the loop, return 'secondLargest' is 34
