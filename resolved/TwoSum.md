# Topic
- Math

## Link
https://leetcode.com/problems/two-sum/solutions/8114876/solution-with-enumerate-by-spamic-jyam


# Code
```python []
class Solution(object):
    def twoSum(self, nums, target):
        """
        :type nums: List[int]
        :type target: int
        :rtype: List[int]
        """
        hash = dict()
        for i,x in enumerate(nums):
            wanted = target - x
            if wanted in hash:
                return [hash[wanted], i]
            else:
                hash[x] = i

        return None
        
```