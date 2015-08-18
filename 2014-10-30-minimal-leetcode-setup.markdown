---
layout: post
title: "Minimal LeetCode Setup"
date: 2014-10-30 20:44:17 -0400
comments: true
categories: programming
---

[LeetCode Online Judge](https://oj.leetcode.com/problems/) is a website that hosts algorithm problems and verifies your solutions. Many of my classmates are working hard on it. While far from finishing, I really enjoyed my clean setup.

The way to do it is having two terminal windows opened side by side. On the left, `mkdir` a new folder to hold all `*.java` and `*.class`. Each problem requires exactly one file so I can stay away from any IDE, which is neat. Then in the right terminal window, say, `vim MaxProductSubarray.java` to start solving a problem:

+ Write the skeleton code.

``` java MaxProductSubarray.java https://oj.leetcode.com/problems/maximum-product-subarray/ Online judge
import java.util.Arrays;
	
// https://oj.leetcode.com/problems/maximum-product-subarray/

public class MaxProductSubarray {
  public static void main(String[] args) {
    test(new int[]{5});
    test(new int[]{-1,3});
    test(new int[]{2,3,-2,4});
    test(new int[]{5,2,0,3,9,0});
    test(new int[]{9,2,4,-3,8,-2,-5});
  }		
  public static int maxProduct(int[] A) {
    return 0;
  }
  public static void test(int[] A) {
    System.out.println(Arrays.toString(A) + " -> " + maxProduct(A));
  }
}
```

+ Before thinking about solutions, write *tests* in `main()`, for I already know the interface of `solution()`. Tests drive you to cover all the edge cases you'd normally overlooked when implementing solutions. Tests inspire me at times.
+ Solve the problem by hand, code the idea and run tests.
+ Take down notes and remember handy Java methods.

When done, in the left terminal use `javac MaxProductSubarray.java` to compile and `java MaxProductSubarray` to execute. `⌘ + 1/2` will also do the switching between terminal windows.

This setup becomes more efficient when I'm better at Vim. Vim has a seriously steep learning curve but [Learn Vim Progressively](http://yannesposito.com/Scratch/en/blog/Learn-Vim-Progressively/) (Chinese version [here](http://coolshell.cn/articles/5426.html)) made me pretty adept at it.

---

->Please ignore. Testing iTunes widget only.<-

-><iframe src="https://widgets.itunes.apple.com/widget.html?c=jp&brc=FFFFFF&blc=FFFFFF&trc=FFFFFF&tlc=FFFFFF&d=The theme song of the extraordinary Japanese TV series Long Wolf and Cub&t=子連れ狼&m=song&e=song&w=250&h=300&ids=374864529&wt=playlist&partnerId=&affiliate_id=&at=&ct=" frameborder=0 style="overflow-x:hidden;overflow-y:hidden;width:250px;height: 300px;border:0px"></iframe><-
