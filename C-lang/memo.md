# matsuyama-memo

# Chapter1-1 データ型を理解する:

C では、整数,浮動小数点数,文字を区別することが重要。

5や8のような整数には小数点がなく、 5.0や8.0のような浮動小数点数には小数点がある。

文字は一重引用符で示される。

例) 5
```c
// Examples
int number = 5; // Integer
float decimal = 5.0; // Floating-point
char character = '5'; // Character

```

### 関数の使用に関する適切な構文:

printf()のような関数を使用する場合は、必ずカンマを使用して書式文字列と変数を区切らないといけない。

カンマがないと float 変数を印刷するときにエラーが発生する。

```c
// Correct use of printf
printf("%f", number);
```

### 変数を正しく宣言する:

変数を宣言するときは、必要なデータ型に基づいて int,float,char などの正しいデータ型キーワードを使用する。

不適切なデータ型は使用しないこと。

```c
// Correct declaration
int age;
float salary;
char letter;
```

### 重要なポイント
1.リテラルはコード内で直接使用される定数値。

2.整数、浮動小数点数、文字を構文によって区別する。

3.printf() のような関数を使用するときは、常に適切な構文を確認する。


<br>
 

# Chapter1-2 フォーマット指定子を正しく指定する:

C プログラミングでデータを正しく表示するには、正しい書式指定子を使用することが重要。

double 変数を表示するときに、float には %f を使用し、double には %lf を使用することを忘れない。

```c
#include <stdio.h>
 
int main() {
    double number = 59.86;
    printf("%lf", number);
    return 0;
}
```

### 出力フォーマットの確保:

複数の変数を印刷したり値を変更したりする場合は、出力が明確であることを確認。

値を区切る新しい行 \n を使用して、出力の読みやすさを向上させることができる。

```c
printf("%d\n", age);
number = 99;
printf("%d\n", number);
```

### 変数の使用における一貫性:

ある変数を別の変数に割り当てるときは、エラーを回避するために、割り当て前に両方の変数が定義され、初期化されていることを確認。

これは、ある変数の値が別の変数に割り当てられているセグメントで示されている。

```c
#include <stdio.h>

int main() {
    int distance = 135;
    int newDistance = 429;
    distance = newDistance;
    printf("%d\n", distance);
    return 0;
}
```

### 重要なポイント
正確な書式指定子を使用してデータ型を一致させる。

出力フォーマットを改善するために　\n　を活用。

割り当てに使用する前に変数を初期化。
