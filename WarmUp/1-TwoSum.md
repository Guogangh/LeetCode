

### 1 - TwoSum

+ [Question](https://leetcode-cn.com/problems/two-sum/)：find indices of two integers in `nums` array which can be added up to `target`

+ Analysis：

  I can use a double loop to solve it.

  O(n<sup>2</sup>) Time, O(1) Space

+ Result：

![image-20190814180014505](../pic/1-TwoSum.png)

+ My Solution：

```python
class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        for i in range(len(nums)):
            for j in range(i):
                if nums[j] + nums[i] == target:
                    return [j, i]
        return [-1, -1]
```

