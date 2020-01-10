---
layout: post
title: LC 344. Reverse String
categories: [top interview, easy]
author: Sarthak Sehgal
excerpt: 
---
Pretty straightforward problem with optimum solution being iterating only till half of the array.
```
class Solution {
public:
    void reverseString(vector<char>& s) {
        for (int i=0; i<s.size()/2; i++) {
            swap(s[i], s[s.size()-i-1]);
        }
    }
};
```
O(n) time and O(1) space.