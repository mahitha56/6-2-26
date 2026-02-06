# 6-2-26
class Solution:
    def findDisappearedNumbers(self, nums: List[int]) -> List[int]:
        
        # missing=[]
        
         n=len(nums)
        
        # for i in range(1,n+1):
        
        #     if i not in nums:
        
        #         missing.append(i)
        
        # return missing
        
         missing = list(set(range(1, n+1)) - set(nums))
         
         return missing

        #   s = set(nums)
        
        # res = []
        
        # for i in range(1, n+1):
        
        #     if i not in s:
        
        #         res.append(i)

        # return res
#

🔥 Dry Run
num	count	max_count
1	1	1
1	2	2
0	0	2
1	1	2
1	2	2
1	3	3
Output → 3
#
# class Solution:
#     def maximumProduct(self, nums: List[int]) -> int:
#         nums.sort()
#         # a=nums[-1]*nums[-2]*nums[-3]
#         # b = nums[0] * nums[1] * nums[-1]
#         # return max(a,b)
#         n=len(nums)
#         res1=nums[n-1]*nums[n-2]*nums[n-3] 
#         res2=nums[n-1]*nums[0]*nums[1] 
#         return max(res1,res2)
class Solution:
    def maximumProduct(self, nums: List[int]) -> int:
        nums.sort()
        n=len(nums)
        res1=nums[n-1]*nums[n-2]*nums[n-3] 
        res2=nums[n-1]*nums[0]*nums[1] 
        return max(res1,res2)




