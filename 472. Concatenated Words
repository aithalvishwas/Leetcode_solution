class Solution {
    public List<String> findAllConcatenatedWordsInADict(String[] words) {
        Set<String> s = new HashSet<>();
        List<String> ans = new ArrayList<>();
        for(String word :words){
            s.add(word);
        }
        for(String word :words){
            if(check(word,s)){
                ans.add(word);
            }
        }
        return ans;
    }
    public static boolean check(String word, Set<String> s){
        for(int i=1;i<word.length();i++){
            String preffix = word.substring(0,i);
            String suffix = word.substring(i,word.length());
            if(s.contains(preffix) && (s.contains(suffix) || check(suffix,s))){
                return true;
            }
        }
        return false;
    }
        
}
