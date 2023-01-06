class Solution {
public:
    int countDigits(int num) {
        vector<int>digit;
        int temp=num;
        while(temp>0){
            digit.push_back(temp%10);
            temp=temp/10;
        }
        int count=0;
        for(int i=0;i<digit.size();i++){
            if(num%digit[i]==0) count++;
            
        }
        return count;
    }
};
