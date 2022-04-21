# Driver Code
nums = [2, 5, 9, 4, 8, 11]
target = 10

class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
  	# search first element in the array
        for i in range (len(nums)):
    	     # search other element in the array
            for j in range(i+1, len(nums)):
                sum = nums[i]+nums[j]
                # if these two elements sum to target, print the pair
                if sum == target:
                    return(i,j)


def twoSum(self, nums, target):
        # create hashmap
        hashMap = {}
        # enumerate() - returns (ith place, ith element)
        for i, n in enumerate(nums):
            # result will be the other number algorithm is finding
            diff = target - n
            # checks if diff is in hashMap
            if diff in hashMap:
                # returns ith index of diff, current ith index
                return hashMap[diff], i
            # appends (ith element, ith index) to the hashMap
            hashMap[n] = i






