# Prof-Thread-Saver
In professional exam of mbbs course, there are several boards of viva. and these are so unpredictable. so There are ways to know how the viva is taken or which type questions are asked. So in facebook group, one makes a post with the title of the exam and other who has took part in exam, write about the exam questions as comment. but  it is done in private facebook group. so can't be share easily.Here is a way to save them:
1. go to the respective post
2. load all the comments
3. Now go to inspect/developer option of the browser then to console. now run the below script to expand all the comments:
```
document.querySelectorAll('a, button, span, div, *[role="button"]').forEach(element => {
  if (/see\s*more/i.test(element.textContent)) {
    element.click();
  }
});
```

4. to load all the reply, run the following script:
```
document.querySelectorAll('a, button, span, div, *[role="button"]').forEach(element => {
  if (/replie/i.test(element.textContent)) {
    element.click();
  }
});
```
5. now press ctrl+p and save it as pdf
