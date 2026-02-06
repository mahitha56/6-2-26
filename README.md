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




