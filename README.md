# git reset --hard --soft的区别

## git的三个区域

![](https://github.com/zhbsdsb/Y/blob/master/8048507-9ea56a58f75ebc00.png?raw=true)

- 1.工作区（working directory）

- 2.暂缓区（stage index）

- 3.历史记录区（history)

## git reset --hard
 
 ![](https://github.com/zhbsdsb/Y/blob/master/%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202018-04-29%20%E4%B8%8B%E5%8D%884.42.01.png?raw=true)
 
- --hard head~1 可以将本地库退回一个版本，而且会重制暂缓区，并且工作区的代码也会退回到那个版本。

## git reset --soft 

![](https://github.com/zhbsdsb/Y/blob/master/%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202018-04-29%20%E4%B8%8B%E5%8D%884.52.16.png?raw=true)

- soft head~1 可以退回一个版本，但只有指针重制到那个版本，工作区代码不变，且将这次提交之后的所有变更都移动到暂存区。


### git log  查看版本  
### git reflog  查看历史版本操作

