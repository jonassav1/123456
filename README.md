# pirma uzduotis https://leetcode.com/problems/length-of-last-word/ Paskutinio zodzio ilgis.
sprendimas mano kompiuteryje o po to jis pritaikytas leet code.
leet code spredimas :

class Solution {
public:
    int lengthOfLastWord(string s) {
        
    
    int i = s.length() - 1; 
    while (i != 0 && !isspace(s[i]))
    {
      --i;
    }
    string paskutiniszodis = s.substr(i+1); 
    
    
    cout <<"Paskutinio zodzio ilgis - " <<paskutiniszodis.size() ;
    
            
    return paskutiniszodis.size();
}
};
