# Introductory Problems

### 1. Weird Algorithm.
    Just take care of overflow, use long long.
  ---
### 2. Missing Number.
    expected sum - sum of inputs
---
### 3. Repetitions. (To find longest repetition in sequence of string)
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


