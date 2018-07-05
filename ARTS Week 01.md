# ARTS Week 01
## Alogrithm
### Two Sum

Given an array of integers, return **indices** of the two numbers such that they add up to a specific target.

You may assume that each input would have **exactly** one solution, and you may not use the same element twice.

```
Given nums = [2, 7, 11, 15], target = 9,

Because nums[0] + nums[1] = 2 + 7 = 9,
return [0, 1]
```
### My Answer

```js
/**
 * @param {number[]} nums
 * @param {number} target
 * @return {number[]}
 */
var twoSum = function(nums, target) {
    for (var i = 0; i < nums.length; i++) {
        for(var j = nums.length - 1; j > i; j--) {
            if (nums[i] + nums[j] === target) {
                return [i, j]
            }
        }
    }
};
```

## Review
[People Who Have “Too Many Interests” Are More Likely To Be Successful According To Research](https://medium.com/the-mission/modern-polymath-81f882ce52db)

这是耗子哥推荐的一篇文章，内容比较长，主要讲了现代社会中成为一个博学的‘多面手’，更有可能获得成功。

文章开头提出数百年中多种语言对于成为一个‘多面手’的警示，然后又列出伊隆. 马斯克、乔布斯、富兰克林、爱迪生等古今中外有影响力的人物都是博学的人。并定义了一个现代的博学者的标准-至少在三个领域胜任，且将其整合到顶级1%技能组合的人。接着引用了各种研究报告，列表了七大优势，为什么成为一个现代的博学者是一个新常态。

最后提出怎么变成一个现代博学者的问题，作者说在他数百小时的研究怎么成为一个博学者和面试博学者，他发现一个关键是心智模式（mental models），文中提到一个著名的“80/20定律”，即在很多领域，你20%的努力会产生你要的结果的80%。我们能利用这个心智模式去提高你生活中每个领域的效率和影响力。

我是赞同人应该有多个领域的涉猎这种观点的，而且合理利用“80/20定律”确实能够让你较高效率的到达一个基本水准。但是在某个领域的擅长需要大量时间的练习，将“知识”转化成“经验”。如何博而有专精？最后我认为，在技术高速发展的现代，确实应该具备能够快速学习的能力。

## Tips
有次，突然想发奇想看看项目都有哪些人提交了commit，能清晰看到每个作者第一次到最后一次提交的时间段就更好了。无奈项目log过长，肉眼看不过来，只能寻求命令帮助。但是对于Git的也只是用过一些基础操作，只能Google之。

> git log --format='%aN' | sort -u

但是列出每个作者时间段的问题还没解决？

## Share
[Git tutorials](https://www.atlassian.com/git/tutorials/git-log)