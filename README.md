# Java言語で学ぶデザインパターン入門 マルチスレッド編

## 環境構築

```sh
$ cat /etc/issue
Ubuntu 20.04 LTS \n \l

$ sudo apt update
$ sudo apt install openjdk-11-jdk
$ which java
/usr/bin/java
```

## 実行

```sh
git clone git@github.com:basd4g/java-design-pattern-multi-thread.git
cd java-design-pattern-multi-thread/hello
javac Hello.java
java Hello
```

## License

### English

The repository's code is based on http://www.hyuki.com/dp/dp2.html written by Hiroshi Yuki.
This software is licensed under zlib/libpng license.

Copyright (c) 2020 Keisuke Nakayama

This software is provided 'as-is', without any express or implied warranty. In no event will the authors be held liable for any damages arising from the use of this software.

Permission is granted to anyone to use this software for any purpose, including commercial applications, and to alter it and redistribute it freely, subject to the following restrictions:

1. The origin of this software must not be misrepresented; you must not claim that you wrote the original software. If you use this software in a product, an acknowledgment in the product documentation would be appreciated but is not required.

2. Altered source versions must be plainly marked as such, and must not be misrepresented as being the original software.

3. This notice may not be removed or altered from any source distribution.

### 日本語

このリポジトリに含まれるコードは、「Java言語で学ぶデザインパターン入門 マルチスレッド編 - 結城浩 著」のサンプルコードを元に一部改変を加えたものである。

元のプログラムは上記の書籍に付属しており、[筆者のページ](http://www.hyuki.com/dp/dp2.html)からも取得できる。

本プログラムは以下の条文で示す zlib/libpng ライセンスに従う。

(以下、[OSG-JP](https://ja.osdn.net/projects/opensource/wiki/licenses%2Fzlib_libpng_license)の条文を元にした参考訳)

Copyright (c) 2020 Keisuke Nakayama

本ソフトウェアは「現状のまま」で、明示であるか暗黙であるかを問わず、何らの保証もなく提供されます。 本ソフトウェアの使用によって生じるいかなる損害についても、作者は一切の責任を負わないものとします。

以下の制限に従う限り、商用アプリケーションを含めて、本ソフトウェアを任意の目的に使用し、自由に改変して再頒布することをすべての人に許可します。

本ソフトウェアの出自について虚偽の表示をしてはなりません。あなたがオリジナルのソフトウェアを作成したと主張してはなりません。 あなたが本ソフトウェアを製品内で使用する場合、製品の文書に謝辞を入れていただければ幸いですが、必須ではありません。
ソースを変更した場合は、そのことを明示しなければなりません。オリジナルのソフトウェアであるという虚偽の表示をしてはなりません。
ソースの頒布物から、この表示を削除したり、表示の内容を変更したりしてはなりません。
