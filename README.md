class Solution {
    public static ArrayList<Integer> commonElements(int a[], int b[]) {
        // Your code here
         ArrayList<Integer> ans = new ArrayList<>();
      Arrays.sort(a);
      Arrays.sort(b);
      int i = 0;
      int j = 0;
      while(i<a.length&&j<b.length){
          if(a[i]==b[j]) {
              ans.add(a[i]);
              i++;
              j++;
      }
      else if (a[i]>b[j])j++;
      else i++;
        
    }
      return ans ;
    }
}
