# non-repeat
{
    public:
    //Function is to check whether two strings are anagram of each other or not.
    bool isAnagram(string a, string b){
        
        // Your code here
        unordered_map<char,int>mp;
        if(a.size()!=b.size())
        {
            return false;
        }
        for(int i=0;i<a.size();i++){
            mp[a[i]]++;
           mp[b[i]]--;
        }
        for(int i=0;i<b.size();i++){
            if(mp[a[i]]!=0)
            
                return false;
            
        }
        
            
                return true;
        
    }

};
