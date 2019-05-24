# Leetcode
每日更新算法题目，欢迎大家踊跃提交
## 5.24
### 1. 有序数组的 Two Sum

[Leetcode ：167. Two Sum II - Input array is sorted (Easy)](https://leetcode.com/problems/two-sum-ii-input-array-is-sorted/description/)

```
Input: numbers={2, 7, 11, 15}, target=9
Output: index1=1, index2=2
```

题目描述：在有序数组中找出两个数，使它们的和为 target。

代码示例：

```java
class Solution {
    public int[] twoSum(int[] numbers, int target) {
    }
}
```
以下剧透警告
---
思路：

```
使用双指针，一个指针指向值较小的元素，一个指针指向值较大的元素。指向较小元素的指针从头向尾遍历，指向较大元素的指针从尾向头遍历。

如果两个指针指向元素的和 sum == target，那么得到要求的结果；
	如果 sum > target，移动较大的元素，使 sum 变小一些；
	如果 sum < target，移动较小的元素，使 sum 变大一些。
```
