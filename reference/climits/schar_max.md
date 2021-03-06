# SCHAR_MAX
* climits[meta header]
* macro[meta id-type]

```cpp
# define SCHAR_MAX implementation-defined
```

## 概要
`signed char` 型が表現できる値の最大値。

値は [`std::numeric_limits`](/reference/limits/numeric_limits.md)`<signed char>::`[`max()`](/reference/limits/numeric_limits/max.md) と等しいが、型が異なり、また `SCHAR_MAX` は `#if` などのプリプロセッサディレクティブで使用できる。

具体的な値は実装依存であるが、127（2<sup>7</sup> - 1）以上であることが規格で定められている。このマクロによって定義される値の型は `int` である。


## 例
```cpp example
#include <climits>
#include <iostream>

int main()
{
  std::cout << SCHAR_MAX << '\n';
}
```


### 出力例
```
127
```

## バージョン
### 言語
- C++03
- C++11


### 処理系
- [Clang](/implementation.md#clang): 3.0, 3.1, 3.2, 3.3, 3.4
- [GCC](/implementation.md#gcc): 4.3.6, 4.4.7, 4.5.3, 4.5.4, 4.6.4, 4.7.3, 4.8.1, 4.8.2, 4.9.0
- [GCC, C++11 mode](/implementation.md#gcc): 4.3.6, 4.4.7, 4.5.3, 4.5.4, 4.6.4, 4.7.3, 4.8.1, 4.8.2, 4.9.0
- [ICC](/implementation.md#icc): ??
- [Visual C++](/implementation.md#visual_cpp): 7.1, 8.0, 9.0, 10.0
