# Introductory Problems

1. ### Weird Algorithm
   Just take care of overflow, use long long

---
3. ### Missing Number.
    expected sum - sum of inputs
---
3. ### Repetitions. (To find longest repetition in sequence of string)
   ```cpp
    // Handle edge case when size = 1
     for(int i = 1; i< s.length(); i++){
        if(s[i] == s[i-1]){
            count++;
            maxim = max(count,maxim);
        }
        else{
            count = 1;
        }
    }
---
4. ### Increasing Array-
    (You want to modify the array so that it is increasing, i.e., every element is at least as large as the previous element. On each move, you may increase the value of 
    any element by one. 
    What is the minimum number of moves required?)?
   
    If a[i] is smaller than a[i-1] then increase a[i-1] till it becomes EQUAL to a[i] for minimum moves.
---
5. ### Permutations
     A permutation of integers 1,2,...,n is called beautiful if there are no adjacent elements whose difference is 1. Construct beautiful permutations:
   
     Sol : Just construct array as 1,5,2,6,3,7,4,8... dpending on number of elements is even or odd. (Hint: First complete 1,2,3,..at alternate positions
     till last like 1, ,2, ,3, ,4then continue from second position alternatively like 1,5,2,6,3,7,4. This can be done by finding number which will ocuupy
     second position).
---
  6. creating strings - next_permutation(s.begin(), s.end()) rearranges the sequence to the next lexicographical permutation and returns true if such a permutation exists; otherwise, it returns false and rearranges the sequence to the smallest permutation.
     If you want to generate all permutations of a sequence in lexicographical order, start with the sorted sequence and repeatedly call next_permutation.

