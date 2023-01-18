class Solution {
    public int maxSubarraySumCircular(int[] nums) {
        int total = 0;
        int max_sum = Integer.MIN_VALUE;
        int temp_max = 0;
        int min_sum = Integer.MAX_VALUE;
        int temp_min=0;
        for(int i=0;i<nums.length;i++){
            total+=nums[i];
            //max
            temp_max+=nums[i];
            if(temp_max>max_sum){
                max_sum=temp_max;
            }
            if(temp_max<0){
                temp_max=0;
            }

            //min
            temp_min+=nums[i];
            if(temp_min<min_sum){
                min_sum=temp_min;
            }
            if(temp_min>0){
                temp_min=0;
            }
        }
        if(total==min_sum){
            return max_sum;
        }
        return Math.max(max_sum,(total-min_sum));
    }
}
