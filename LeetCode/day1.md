# Day 1

2023-2-6

# 1. 两数之和

给定一个整数数组 nums 和一个整数目标值 target，请你在该数组中找出 和为目标值 target 的那 两个 整数，并返回它们的数组下标。

## My Code

枚举所有可能进行计算

```
class Solution {
    public int[] twoSum(int[] nums, int target) {
    for (int i =0 ;i< nums.length ;i++){
        for ( int j = i+ 1 ; j< nums.length; j++  ) {
            if ( nums[i] + nums[j] == target ) {
                int[] result = {i,j};
                return result;
            }
        }
    }
    return null;
    }
}
```

## Best Answer
