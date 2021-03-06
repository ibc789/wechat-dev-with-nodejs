# 异步流程控制

> 全异步就应该有全异步的思维方式

## 什么异步流程控制

大家都知道流程控制是程序里最常见的用于控制逻辑的统称。那为什么在Node.js里就变成了异步流程控制了呢？

这和Node.js本身都是异步的有关，如果每个函数都是异步的，性能好了，后遗症就是callback hell，为了解决callbackhell问题，在Node.js用于流程控制的部分成为异步流程控制。

Node.js从一开始就破旧立新，导致它经常被黑的callbackhell问题。但也正是验证的callbackhell，使得Node.js里的异步流程控制发展的特别快，比如thunk实现，promise/a+规范的落地，es6中的generator和为了generator而写的co模块，以及目前最看好的async函数。各种Node.js的辅助模块更是多的数不清，比如async.js这样的好模块非常多。

可是这样说，掌握了Node.js里的异步流程控制，你就掌握了一半以上的Node.js了

## 本章主要内容

那么，Node.js中的异步流程控制发展的过快，也还是会给诟病，“你太复杂，如何如何。。。”

事实上，这都是不了解不负责的人讲的话，本章视图去繁就简，希望能够让大家了解简单易用，拨云见日的一面。

主要讲3个部分

- Promise
- Generator/yield
- Async/await

最后根据这些内容，推导出我们要学习的重点，避免霰弹式的学习。
