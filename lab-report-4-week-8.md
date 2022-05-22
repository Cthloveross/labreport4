# Lab Report 4 
### Name: Tianhao Chen(A16875083)

---

## Links to markdown-parser repositories
[markdown-parser](https://github.com/Cthloveross/markdown-parse)<br>
[Reviewed-markdown-parser](https://github.com/Cthloveross/reviewedmarkdownparse)

---



## Expeted results (using VScode preview function)
#### snippet1
![image](snip1show.png)
#### snippet2
![image](snip2show.png)
#### snippet3
![image](snip3show.png)

## Here is the code for tests in MarkdownParseTest.java
#### snippet1
![image](implement-snip1.png)
#### snippet2
![image](implement-snip2.png)
#### snippet3
![image](implement-snip3.png)

## Here is the output of running tests.
#### here is my implementation by using junit
![image](junit-mine.png)

#### here is reviewed implementation by using junit
![image](junit-review.png)

## My implementation for failures
#### Failed Snippet1
![image](failsnip1-mine.png)
#### Failed Snippet2
![image](failsnip2-mine.png)
#### Failed Snippet3
![image](failsnip3-mine.png)

## Reviewed implementation for failures
#### Failed Snippet1
![image](failsnip1-review.png)
#### Failed Snippet2
![image](failsnip2-review.png)
#### Failed Snippet3
![image](failsnip3-review.png)

---

## Questions:

Answer for question 1: From my perspective, I think the problem for snippet1 failure can be fixed in 10 lines because it is just a small mistake. Now it considers ```url.com``` as a valid link, but ```ucsd.edu``` as on invalid one. For ```url.com```,I just need to add one ```if statement``` to check if there is an openbracket is at the beginning. For ```ucsd.edu```,I just need to add one ```if statement``` to check if a backtick is the previous character.

Answer for question 2: From my perspective, I think the problem for snippet1 failure maynot be fixed in 10 lines because we have to consider too many situations. The problem we have now is that index is out of bounds. For, example, I can check if there exists additional brackets, but the problem has too many combinations, so 10 line might not be enough for me.

Answer for question 3: Similar to Snippet2, I don't think that a small change within 10 lines can fix the problem I have now, and the problem is also index is out of bound. To fix the problem, I have to check if there is a missing ```openbracket```, or ```closeparen```, these changes may take more than 10 lines.
