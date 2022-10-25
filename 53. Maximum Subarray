class Solution:
    def maxSubArray(self, nums: List[int]) -> int:
        cur_sub = max_sum = nums[0]
        for num in nums[1:]:
            #-2    =  max (1,   -2+1=-1) =1 [-2,1][1]
            # 1 = max (-3,   1 + -3=-2) = = -2 [1,-3][-3]
            #-2 = max (4,    -2+4=2)=4    [-2,4][4]
            #4 = max (-1,    4+-1=3)=3
            #3 = max (2,    3+2=5)=5
            #5 = max (1,    5+1)=6
            #6 = max (-5,   -5+6=1)=1
            #1 = max (4,  4+1=5)=5
            cur_sub = max(num, cur_sub+num)
            max_sum = max(max_sum,cur_sub)
        return max_sum
        
        
