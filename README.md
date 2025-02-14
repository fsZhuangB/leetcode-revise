## 相关介绍
这是一个简易的LeetCode自动统计程序, 可自动统计最近提交通过的题目, 并以Markdown的形式展示相关的数据。
根据个人需求, 我只重点获取**提交次数**和**重刷次数**这两个指标, 目的是为了更好地辅助做题。
## 使用教程
1. Fork本仓库
2. 配置GitHub Actions所需的参数
    - 点击仓库下的Settings->Secrets->New repository secret, 分别添加以下secret
        - Name:LEETCODE_EMAIL  Value:你的LeetCode账号
        - Name:LEETCODE_PASSWORD  Value:你的LeetCode密码
    - 点击[tokens](https://github.com/settings/tokens)->Generate new token
        - Note:GITHUB_TOKEN
        - Select scopes:建议全部勾选
    - 修改[action.yml](.github/workflows/action.yml)文件的第`42行`, 将`email`更改为你的GitHub邮箱地址
    - 修改[action.yml](.github/workflows/action.yml)文件的第`43行`, 将`name`更改为你的GitHub用户名
3. 默认配置为12小时更新一次，可根据需求修改[action.yml](.github/workflows/action.yml)文件的第`6行`
## 补充说明
如有其他需求, 欢迎提交PR。


> 重刷次数的计算规则为: 累计所有提交通过且互为不同一天的记录次数

| 最近提交时间 | 题目 | 题目难度 | 提交次数| 重刷次数 |
| ---- | ---- | ---- | ---- | ---- |
| 2022-01-01 12:35 | [#2022 将一维数组转变成二维数组](https://leetcode-cn.com/problems/convert-1d-array-into-2d-array) | EASY | 2 | 1 |
| 2022-01-01 11:23 | [#75 颜色分类](https://leetcode-cn.com/problems/sort-colors) | MEDIUM | 1 | 1 |
| 2022-01-01 11:18 | [#80 删除有序数组中的重复项 II](https://leetcode-cn.com/problems/remove-duplicates-from-sorted-array-ii) | MEDIUM | 1 | 1 |
| 2022-01-01 10:42 | [#15 三数之和](https://leetcode-cn.com/problems/3sum) | MEDIUM | 11 | **4** |
| 2022-01-01 09:49 | [#11 盛最多水的容器](https://leetcode-cn.com/problems/container-with-most-water) | MEDIUM | 3 | **2** |
| 2022-01-01 09:43 | [#26 删除有序数组中的重复项](https://leetcode-cn.com/problems/remove-duplicates-from-sorted-array) | EASY | 14 | **5** |
| 2021-12-31 08:27 | [#226 翻转二叉树](https://leetcode-cn.com/problems/invert-binary-tree) | EASY | 4 | **2** |
| 2021-12-31 08:14 | [#3 无重复字符的最长子串](https://leetcode-cn.com/problems/longest-substring-without-repeating-characters) | MEDIUM | 7 | **5** |
| 2021-12-31 08:02 | [#209 长度最小的子数组](https://leetcode-cn.com/problems/minimum-size-subarray-sum) | MEDIUM | 18 | **6** |
| 2021-12-30 18:43 | [#383 赎金信](https://leetcode-cn.com/problems/ransom-note) | EASY | 1 | 1 |
| 2021-12-30 18:01 | [#102 二叉树的层序遍历](https://leetcode-cn.com/problems/binary-tree-level-order-traversal) | MEDIUM | 1 | 1 |
| 2021-12-30 17:41 | [#94 二叉树的中序遍历](https://leetcode-cn.com/problems/binary-tree-inorder-traversal) | EASY | 4 | **3** |
| 2021-12-30 17:16 | [#374 猜数字大小](https://leetcode-cn.com/problems/guess-number-higher-or-lower) | EASY | 1 | 1 |
| 2021-12-30 17:12 | [#278 第一个错误的版本](https://leetcode-cn.com/problems/first-bad-version) | EASY | 1 | 1 |
| 2021-12-30 16:53 | [#34 在排序数组中查找元素的第一个和最后一个位置](https://leetcode-cn.com/problems/find-first-and-last-position-of-element-in-sorted-array) | MEDIUM | 13 | **3** |
| 2021-12-28 12:32 | [#76 最小覆盖子串](https://leetcode-cn.com/problems/minimum-window-substring) | HARD | 1 | 1 |
| 2021-12-28 11:37 | [#219 存在重复元素 II](https://leetcode-cn.com/problems/contains-duplicate-ii) | EASY | 5 | **2** |
| 2021-12-28 11:05 | [#217 存在重复元素](https://leetcode-cn.com/problems/contains-duplicate) | EASY | 2 | **2** |
| 2021-12-27 22:57 | [#1 两数之和](https://leetcode-cn.com/problems/two-sum) | EASY | 13 | **7** |
| 2021-12-26 10:35 | [#2119 反转两次的数字](https://leetcode-cn.com/problems/a-number-after-a-double-reversal) | EASY | 1 | 1 |
| 2021-12-26 08:31 | [#25 K 个一组翻转链表](https://leetcode-cn.com/problems/reverse-nodes-in-k-group) | HARD | 2 | **2** |
| 2021-12-25 08:44 | [#206 反转链表](https://leetcode-cn.com/problems/reverse-linked-list) | EASY | 14 | **8** |
| 2021-12-25 08:28 | [#148 排序链表](https://leetcode-cn.com/problems/sort-list) | MEDIUM | 7 | **2** |
| 2021-12-24 13:49 | [#147 对链表进行插入排序](https://leetcode-cn.com/problems/insertion-sort-list) | MEDIUM | 5 | **3** |
| 2021-12-23 10:39 | [#21 合并两个有序链表](https://leetcode-cn.com/problems/merge-two-sorted-lists) | EASY | 16 | **9** |
| 2021-12-21 11:12 | [#28 实现 strStr()](https://leetcode-cn.com/problems/implement-strstr) | EASY | 1 | 1 |
| 2021-12-20 15:11 | [#54 螺旋矩阵](https://leetcode-cn.com/problems/spiral-matrix) | MEDIUM | 2 | 1 |
| 2021-12-20 12:20 | [#剑指 Offer 58 - II 左旋转字符串](https://leetcode-cn.com/problems/zuo-xuan-zhuan-zi-fu-chuan-lcof) | EASY | 2 | 1 |
| 2021-12-20 11:48 | [#151 翻转字符串里的单词](https://leetcode-cn.com/problems/reverse-words-in-a-string) | MEDIUM | 2 | 1 |
| 2021-12-20 10:28 | [#541 反转字符串 II](https://leetcode-cn.com/problems/reverse-string-ii) | EASY | 1 | 1 |
| 2021-12-20 09:55 | [#2109 向字符串添加空格](https://leetcode-cn.com/problems/adding-spaces-to-a-string) | MEDIUM | 4 | **2** |
| 2021-12-19 12:58 | [#2110 股票平滑下跌阶段的数目](https://leetcode-cn.com/problems/number-of-smooth-descent-periods-of-a-stock) | MEDIUM | 5 | 1 |
| 2021-12-19 10:33 | [#2108 找出数组中的第一个回文字符串](https://leetcode-cn.com/problems/find-first-palindromic-string-in-the-array) | EASY | 1 | 1 |
| 2021-12-18 10:29 | [#61 旋转链表](https://leetcode-cn.com/problems/rotate-list) | MEDIUM | 12 | **3** |
| 2021-12-17 08:37 | [#86 分隔链表](https://leetcode-cn.com/problems/partition-list) | MEDIUM | 2 | **2** |
| 2021-12-16 10:48 | [#707 设计链表](https://leetcode-cn.com/problems/design-linked-list) | MEDIUM | 11 | **3** |
| 2021-12-15 10:43 | [#142 环形链表 II](https://leetcode-cn.com/problems/linked-list-cycle-ii) | MEDIUM | 4 | **2** |
| 2021-12-15 10:07 | [#面试题 02.07 链表相交](https://leetcode-cn.com/problems/intersection-of-two-linked-lists-lcci) | EASY | 2 | **2** |
| 2021-12-14 13:43 | [#24 两两交换链表中的节点](https://leetcode-cn.com/problems/swap-nodes-in-pairs) | MEDIUM | 1 | 1 |
| 2021-12-13 09:37 | [#2104 子数组范围和](https://leetcode-cn.com/problems/sum-of-subarray-ranges) | MEDIUM | 2 | **2** |
| 2021-12-13 08:41 | [#2099 找到和最大的长度为 K 的子序列](https://leetcode-cn.com/problems/find-subsequence-of-length-k-with-the-largest-sum) | EASY | 12 | **2** |
| 2021-12-12 12:08 | [#2105 给植物浇水 II](https://leetcode-cn.com/problems/watering-plants-ii) | MEDIUM | 6 | 1 |
| 2021-12-12 10:57 | [#2103 环和杆](https://leetcode-cn.com/problems/rings-and-rods) | EASY | 1 | 1 |
| 2021-12-11 09:43 | [#19 删除链表的倒数第 N 个结点](https://leetcode-cn.com/problems/remove-nth-node-from-end-of-list) | MEDIUM | 1 | 1 |
| 2021-12-10 11:23 | [#82 删除排序链表中的重复元素 II](https://leetcode-cn.com/problems/remove-duplicates-from-sorted-list-ii) | MEDIUM | 4 | **2** |
| 2021-12-10 10:57 | [#83 删除排序链表中的重复元素](https://leetcode-cn.com/problems/remove-duplicates-from-sorted-list) | EASY | 5 | **4** |
| 2021-12-10 10:42 | [#203 移除链表元素](https://leetcode-cn.com/problems/remove-linked-list-elements) | EASY | 3 | **2** |
| 2021-12-09 13:26 | [#141 环形链表](https://leetcode-cn.com/problems/linked-list-cycle) | EASY | 11 | **5** |
| 2021-12-09 13:01 | [#237 删除链表中的节点](https://leetcode-cn.com/problems/delete-node-in-a-linked-list) | EASY | 1 | 1 |
| 2021-12-07 11:22 | [#16 最接近的三数之和](https://leetcode-cn.com/problems/3sum-closest) | MEDIUM | 4 | 1 |
| 2021-12-06 09:05 | [#剑指 Offer 05 替换空格](https://leetcode-cn.com/problems/ti-huan-kong-ge-lcof) | EASY | 1 | 1 |
| 2021-12-06 08:28 | [#27 移除元素](https://leetcode-cn.com/problems/remove-element) | EASY | 8 | **4** |
| 2021-12-06 08:00 | [#18 四数之和](https://leetcode-cn.com/problems/4sum) | MEDIUM | 6 | **2** |
| 2021-12-04 10:23 | [#977 有序数组的平方](https://leetcode-cn.com/problems/squares-of-a-sorted-array) | EASY | 2 | 1 |
| 2021-12-03 07:56 | [#202 快乐数](https://leetcode-cn.com/problems/happy-number) | EASY | 2 | 1 |
| 2021-12-03 07:33 | [#49 字母异位词分组](https://leetcode-cn.com/problems/group-anagrams) | MEDIUM | 2 | **2** |
| 2021-12-02 10:44 | [#349 两个数组的交集](https://leetcode-cn.com/problems/intersection-of-two-arrays) | EASY | 2 | 1 |
| 2021-12-02 10:19 | [#242 有效的字母异位词](https://leetcode-cn.com/problems/valid-anagram) | EASY | 2 | 1 |
| 2021-12-01 10:32 | [#2091 从数组中移除最大值和最小值](https://leetcode-cn.com/problems/removing-minimum-and-maximum-from-array) | MEDIUM | 6 | 1 |
| 2021-12-01 09:49 | [#643 子数组最大平均数 I](https://leetcode-cn.com/problems/maximum-average-subarray-i) | EASY | 8 | 1 |
| 2021-11-30 09:59 | [#560 和为 K 的子数组](https://leetcode-cn.com/problems/subarray-sum-equals-k) | MEDIUM | 9 | 1 |
| 2021-11-28 15:18 | [#2090 半径为 k 的子数组平均值](https://leetcode-cn.com/problems/k-radius-subarray-averages) | MEDIUM | 2 | 1 |
| 2021-11-28 14:58 | [#303 区域和检索 - 数组不可变](https://leetcode-cn.com/problems/range-sum-query-immutable) | EASY | 2 | 1 |
| 2021-11-28 14:33 | [#1480 一维数组的动态和](https://leetcode-cn.com/problems/running-sum-of-1d-array) | EASY | 2 | 1 |
| 2021-11-28 10:43 | [#2089 找出数组排序后的目标下标](https://leetcode-cn.com/problems/find-target-indices-after-sorting-array) | EASY | 1 | 1 |
| 2021-11-27 09:27 | [#1137 第 N 个泰波那契数](https://leetcode-cn.com/problems/n-th-tribonacci-number) | EASY | 1 | 1 |
| 2021-11-26 10:29 | [#509 斐波那契数](https://leetcode-cn.com/problems/fibonacci-number) | EASY | 4 | 1 |
| 2021-11-26 08:24 | [#343 整数拆分](https://leetcode-cn.com/problems/integer-break) | MEDIUM | 5 | **3** |
| 2021-11-23 10:33 | [#704 二分查找](https://leetcode-cn.com/problems/binary-search) | EASY | 2 | 1 |
| 2021-11-22 08:13 | [#2080 区间内查询数字的频率](https://leetcode-cn.com/problems/range-frequency-queries) | MEDIUM | 6 | 1 |
| 2021-11-21 11:52 | [#2079 给植物浇水](https://leetcode-cn.com/problems/watering-plants) | MEDIUM | 1 | 1 |
| 2021-11-21 10:38 | [#2078 两栋颜色不同且距离最远的房子](https://leetcode-cn.com/problems/two-furthest-houses-with-different-colors) | EASY | 1 | 1 |
| 2021-11-20 17:53 | [#225 用队列实现栈](https://leetcode-cn.com/problems/implement-stack-using-queues) | EASY | 2 | 1 |
| 2021-11-20 09:36 | [#1047 删除字符串中的所有相邻重复项](https://leetcode-cn.com/problems/remove-all-adjacent-duplicates-in-string) | EASY | 3 | **2** |
| 2021-11-19 10:43 | [#232 用栈实现队列](https://leetcode-cn.com/problems/implement-queue-using-stacks) | EASY | 1 | 1 |
| 2021-11-18 10:37 | [#63 不同路径 II](https://leetcode-cn.com/problems/unique-paths-ii) | MEDIUM | 3 | 1 |
| 2021-11-18 09:59 | [#5 最长回文子串](https://leetcode-cn.com/problems/longest-palindromic-substring) | MEDIUM | 15 | **3** |
| 2021-11-16 12:07 | [#62 不同路径](https://leetcode-cn.com/problems/unique-paths) | MEDIUM | 2 | 1 |
| 2021-11-16 11:19 | [#746 使用最小花费爬楼梯](https://leetcode-cn.com/problems/min-cost-climbing-stairs) | EASY | 4 | **2** |
| 2021-11-14 10:24 | [#70 爬楼梯](https://leetcode-cn.com/problems/climbing-stairs) | EASY | 4 | **2** |
| 2021-11-13 10:39 | [#344 反转字符串](https://leetcode-cn.com/problems/reverse-string) | EASY | 1 | 1 |
| 2021-11-12 11:09 | [#20 有效的括号](https://leetcode-cn.com/problems/valid-parentheses) | EASY | 12 | **5** |
| 2021-11-06 15:38 | [#14 最长公共前缀](https://leetcode-cn.com/problems/longest-common-prefix) | EASY | 4 | **2** |
| 2021-11-05 21:49 | [#13 罗马数字转整数](https://leetcode-cn.com/problems/roman-to-integer) | EASY | 4 | **2** |
| 2021-11-04 17:49 | [#6 Z 字形变换](https://leetcode-cn.com/problems/zigzag-conversion) | MEDIUM | 2 | 1 |
| 2021-11-02 18:56 | [#7 整数反转](https://leetcode-cn.com/problems/reverse-integer) | MEDIUM | 8 | **2** |
| 2021-10-31 20:07 | [#2 两数相加](https://leetcode-cn.com/problems/add-two-numbers) | MEDIUM | 1 | 1 |
| 2020-05-11 11:20 | [#118 杨辉三角](https://leetcode-cn.com/problems/pascals-triangle) | EASY | 1 | 1 |
| 2020-05-10 09:21 | [#35 搜索插入位置](https://leetcode-cn.com/problems/search-insert-position) | EASY | 4 | **2** |
| 2020-05-09 19:39 | [#66 加一](https://leetcode-cn.com/problems/plus-one) | EASY | 5 | 1 |
| 2020-05-03 17:34 | [#53 最大子数组和](https://leetcode-cn.com/problems/maximum-subarray) | EASY | 1 | 1 |
| 2020-05-03 16:39 | [#104 二叉树的最大深度](https://leetcode-cn.com/problems/maximum-depth-of-binary-tree) | EASY | 3 | **2** |
| 2020-05-03 15:38 | [#剑指 Offer 18 删除链表的节点](https://leetcode-cn.com/problems/shan-chu-lian-biao-de-jie-dian-lcof) | EASY | 4 | **2** |
| 2020-05-02 10:05 | [#面试题 02.06 回文链表](https://leetcode-cn.com/problems/palindrome-linked-list-lcci) | EASY | 5 | 1 |
| 2020-05-02 09:25 | [#9 回文数](https://leetcode-cn.com/problems/palindrome-number) | EASY | 15 | **3** |
| 2020-04-28 08:21 | [#88 合并两个有序数组](https://leetcode-cn.com/problems/merge-sorted-array) | EASY | 12 | **2** |
| 2020-04-24 09:52 | [#剑指 Offer 24 反转链表](https://leetcode-cn.com/problems/fan-zhuan-lian-biao-lcof) | EASY | 1 | 1 |
| 2019-10-24 09:34 | [#876 链表的中间结点](https://leetcode-cn.com/problems/middle-of-the-linked-list) | EASY | 2 | 1 |
| 2019-10-17 20:43 | [#234 回文链表](https://leetcode-cn.com/problems/palindrome-linked-list) | EASY | 3 | 1 |
| 2019-09-27 09:16 | [#160 相交链表](https://leetcode-cn.com/problems/intersection-of-two-linked-lists) | EASY | 2 | 1 |
| 2019-09-25 10:07 | [#92 反转链表 II](https://leetcode-cn.com/problems/reverse-linked-list-ii) | MEDIUM | 2 | **2** |
