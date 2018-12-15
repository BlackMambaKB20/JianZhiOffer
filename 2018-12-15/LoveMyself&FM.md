import java.util.Arrays;
public class Solution {
    public int MoreThanHalfNum_Solution(int [] array) {
        Arrays.sort(array);
        int len=array.length;
        int num=array[len/2];
        int count=0;
        for(int i=0;i<array.length;i++){
            if(array[i]==num){
                count++;
            }
        }
        return count>(len/2)?num:0;
    }
}
