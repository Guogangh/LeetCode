**66 - 加一**

- [问题](https://leetcode-cn.com/problems/plus-one/submissions/)给定整数组成非空数组，在该数基础上加一，最高位置于数组首位

- 分析：

  可以使用循环解决。

- 结果：

  ![](/Users/jxtx/Library/Application Support/typora-user-images/image-20190815231131723.png)

- 我的解决方案：

  ```
  public static int[] plusOne(int[] digits) {
          for (int i = digits.length -1; i >= 0; i--) {
              digits[i]++;
              digits[i] = digits[i] % 10;
              if (digits[i] != 0)
                  return digits;
          }
          digits = new int[digits.length + 1];
          digits[0] = 1;
          return digits;
      }
  ```

  

  

  
