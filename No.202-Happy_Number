/*判斷過程中是否有重複元素出現，若有則立即停止(實際例子顯示若有4出現也非快樂數)*/
class Solution {
    public boolean isHappy(int n) {
        Set<Integer> set = new HashSet<>();
        int count =0;
        while(n!=1){
            while(n!=0){
                count = count+ (n%10)*(n%10);
                n /= 10;
            }
            
            if(!set.add(count)){
                return false;
            }  
            n = count;
            count = 0;
        }   
        // n=1 時能出來
        return true;
    }
        
/*        int k=0;
        while(n!=1)
        {
            if(n==4)
                return false;
            while(n!=0)
            {
                k=k+n%10*(n%10);
                n/=10;
            }
            n=k;
            k=0;
        }
        return true;
        }*/
}
