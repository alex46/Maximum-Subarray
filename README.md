Maximum-Subarray
================


public class Solution {
    public int maxSubArray(int[] A) {
        // Start typing your Java solution below
        // DO NOT write main() function
     
     int sum = Integer.MIN_VALUE;
     int subsum = 0;
     
     for(int i = 0; i < A.length; i++){
         subsum += A[i];
         
         if(subsum > sum){
             sum = subsum;
         }
         
         if(subsum <0){
             subsum = 0;
         }
         
     }
     
     return sum;
       
    }
}
