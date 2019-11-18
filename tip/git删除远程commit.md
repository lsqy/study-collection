# git删除远程commit

```
//git删除远程提交（确保还没其他人提交之前，进行强制回滚）
//(数字代表回退几个版本)
git reset --hard HEAD~2
//强制覆盖
git push -f
```