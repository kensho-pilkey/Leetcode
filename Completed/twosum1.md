# Two Sum not sorted:

class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        box = {}
        for i, num in enumerate(nums):
            searchFor = target - num
            if searchFor in box:
                return [box[searchFor], i]
            box[num] = i


# TC: O(n)
# SC: O(n)
