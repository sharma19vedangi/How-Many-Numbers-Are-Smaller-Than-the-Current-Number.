# How-Many-Numbers-Are-Smaller-Than-the-Current-Number.
#Array Leetcode Problem Solution
class Solution {
    public int[] smallerNumbersThanCurrent(int[] nums) {
        int a[]=new int[nums.length];
        int count;
        for(int i=0;i<nums.length;i++)
        {
            count=0;
            for(int j=0;j<nums.length;j++)
            {
                if(j!=i)
                {
                    if(nums[i]>nums[j])
                      {
                        count=count+1;
                      }
                }
                
            }
            a[i]=count;
        }
        return a;
    }
}
