class Solution {

    public boolean containsDuplicate(int[] nums) {

      Set<Integer> set = new HashSet<>();
      for(int i = 0; i < nums.length; i++) {
          if(set.contains(nums[i])) {
              return true;
          } else {
              set.add(nums[i]);
          }
      }
      return false;

        
    }
    
}

/*
Utilize Set or Hashset as arraylist when arraylist is too slow / time exceeds the expectation
Average runtime for hashSet is O(1).
*/
