# LeetCode_question_1672

class Solution {
    public int maximumWealth(int[][] accounts) {
        int maxCount = 0;

        for(int[] account:accounts){
            int count = 0;
            for(int i=0; i<account.length; i++){
                count = count + account[i];
            }
            maxCount = Math.max(maxCount, count);
        }
        return maxCount;
    }
}
