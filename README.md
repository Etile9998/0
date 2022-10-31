# �����ϴٰ� �ñ��� �͵� ���� �غ��� �뵵

## Markdown ����
* [������](https://www.markdowntutorial.com/kr/)

## JAVA
* [public class�� �׳� class �� ����1](https://stackoverflow.com/questions/16779245/what-is-the-difference-between-public-class-and-just-class)
* [public class�� �׳� class �� ����2](https://stackoverflow.com/questions/215497/what-is-the-difference-between-public-protected-package-private-and-private-in)

|Modifier|Class|Package|Subclass(same pkg)|Subclass(diff pkg)|World|
|---|---|---|---|---|---|
|public|Y|Y|Y|Y|Y|
|protected|Y|Y|Y|Y|N|
|*no modifier*|Y|Y|Y|N|N|
|private|Y|N|N|N|N|

* [static Ŭ������ ���ӻ�](https://stackoverflow.com/questions/7486012/static-classes-in-java)
  * [Ex: Math class�� PI, E](https://hg.openjdk.java.net/jdk/jdk11/file/1ddf9a99e4ad/src/java.base/share/classes/java/lang/Math.java)
  ```
  // import java.lang.Math;
  public static final double E = 2.718281828459045;
  public static final double PI = 3.141592653589793;
  ```

* [Java�� main �޼ҵ��� �ǹ�(public, static)](https://stackoverflow.com/questions/52803874/please-explain-every-element-of-java-main-public-static-void-mainstring-arg)
```
public : �ֿܼ��� ������ �� �ְ�
static : ���α׷� ����� �ٷ� �޸𸮿� �Ҵ��ϱ� ���ؼ�
void : ��ȯ���� ����
main : main �̸�
```

* String Ŭ������ �̿��ؼ� ���ڿ� ������ �� �� ���ڿ� �ν��Ͻ��� ����ؼ� ���ܳ��� ���� �ٶ����� ������ �ƴϴ�! ���� �� ��쿡�� ���ڿ� �ν��Ͻ� ������ �ּ�ȭ�ذ��� ���ڿ��� ������ �� �ֵ��� StringBuilder Ŭ������ ����ϴ� ���� ����!

* [StringBuffer�� StringBuilder�� ����
](https://stackoverflow.com/questions/355089/difference-between-stringbuilder-and-stringbuffer)
```
package note;

public class Foo {
    public static void main(String[] args) {
        int N = 77777777;
        long t;

        {
            StringBuffer sb = new StringBuffer();
            t = System.currentTimeMillis();
            for (int i = N; i-- > 0;) {
                sb.append("");
            }
            System.out.println(System.currentTimeMillis() - t); // 1149ms
        }

        {
            StringBuilder sb = new StringBuilder();
            t = System.currentTimeMillis();
            for (int i = N; i > 0; i--) {
                sb.append("");
            }
            System.out.println(System.currentTimeMillis() - t); // 84ms
        }
    }
}
```
```
�⺻������ �ӵ��� ���̰� �ְ�, �����忡�� ���ư��°� �ƴѰ��� ���̰� �ִ�.
1149
84
```

* [@Override ������̼�](https://velog.io/@pearl0725/Override-%EC%96%B4%EB%85%B8%ED%85%8C%EC%9D%B4%EC%85%98%EC%9D%98-%EC%9D%98%EB%AF%B8%EC%99%80-%EC%82%AC%EC%9A%A9-%EC%9D%B4%EC%9C%A0%EB%8A%94-%EB%AC%B4%EC%97%87%EC%9D%BC%EA%B9%8C)

* [int[] array�� int array[]�� ����](https://stackoverflow.com/questions/129178/difference-between-int-array-and-int-array)
```
int[] foo, bar; // foo, bar = array
int foo[], bar; // foo = array, bar = int
```

* [���� �򰥸� �� �ִ� �� : �����ε� vs �������̵�](https://stackoverflow.com/questions/154577/polymorphism-vs-overriding-vs-overloading)
```
�����ε� : �Ű������� �ٸ� ��
�������̵� : �θ�Ŭ������ �޼ҵ�� ���� �̸��� �޼ҵ带 �������Ͽ� ���� ��
```

* [�ڹٿ��� super.super.method()�� ��� ���� �ʴ� ����](https://stackoverflow.com/questions/586363/why-is-super-super-method-not-allowed-in-java)
```
ĸ��ȭ
```

* [abstract interface ���� ����](https://stackoverflow.com/questions/7202616/java-abstract-interface)

* [interface �� abstract class �� ����](https://stackoverflow.com/questions/1913098/what-is-the-difference-between-an-interface-and-abstract-class/1913185#1913185)

* [�޸� ���� 1](https://docs.oracle.com/javase/specs/jvms/se15/html/jvms-2.html#jvms-2.5.4)

* [�޸� ���� 2](https://stackoverflow.com/questions/79923/what-and-where-are-the-stack-and-heap?page=1&tab=scoredesc#tab-top)


## PS/CP
* [Tip](https://cses.fi/book/book.pdf)
* [����](https://drive.google.com/file/d/1J2x8pIYQ3MXANgvzOgBciWd3d79j_Exa/view)
* [USACO GUIDE](https://usaco.guide/)
* [��� ����](https://codeforces.com/blog/entry/85668)