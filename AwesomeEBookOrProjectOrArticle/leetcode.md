## leetcode

### 1、两数相加

> 给定一个整数数组 nums 和一个目标值 target，请你在该数组中找出和为目标值的那 两个 整数，并返回他们的数组下标。你可以假设每种输入只会对应一个答案。但是，你不能重复利用这个数组中同样的元素。

```

/**
 * @param {number[]} nums
 * @param {number} target
 * @return {number[]}
 */
var twoSum = function(nums, target) {
    var hashMap = {}; // 声明一个对象
    for(var i = 0; i < nums.length; i++) {
        var val = nums[i];
        var delta = target - val;
        var deltaIdx = hashMap[delta];
        if(deltaIdx !== undefined && deltaIdx !== i) {
            return [deltaIdx, i];
        }
        hashMap[val] = i;
    }
    return [];
};

var twoSum2 = function(nums, target) {
  for(var i = 0; i < nums.length; i++) {
    var val = nums[i];
    for (var j = i + 1; j < nums.length; j++) {
      if (val + nums[j] === target) {
        return [i, j]
      }
    }
  }
  return [];
};

```