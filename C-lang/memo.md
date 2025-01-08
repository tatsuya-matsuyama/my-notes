#memo

#Chapter1 データ型を理解する:

C では、整数,浮動小数点数,文字を区別することが重要。 5や8のような整数には小数点がなく、 5.0や8.0のような浮動小数点数には小数点がある。
文字は一重引用符で示される 

例) 5

// Examples
int number = 5; // Integer
float decimal = 5.0; // Floating-point
char character = '5'; // Character


## 関数の使用に関する適切な構文:

printf()のような関数を使用する場合は、必ずカンマを使用して書式文字列と変数を区切らないといけない。
カンマがないと float 変数を印刷するときにエラーが発生する。

// Correct use of printf
printf("%f", number);


## 変数を正しく宣言する:

変数を宣言するときは、必要なデータ型に基づいて int,float,char などの正しいデータ型キーワードを使用する。
不適切なデータ型は使用しないこと。

// Correct declaration
int age;
float salary;
char letter;


## 重要なポイント
1.リテラルはコード内で直接使用される定数値。
2.整数、浮動小数点数、文字を構文によって区別する。
3.printf() のような関数を使用するときは、常に適切な構文を確認する。
