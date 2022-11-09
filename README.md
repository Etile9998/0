# 공부하다가 궁금한 것들 정리 해보는 용도

## Markdown 문법
* [익히기](https://www.markdowntutorial.com/kr/)

## JAVA
* [public class와 그냥 class 의 차이1](https://stackoverflow.com/questions/16779245/what-is-the-difference-between-public-class-and-just-class)
* [public class와 그냥 class 의 차이2](https://stackoverflow.com/questions/215497/what-is-the-difference-between-public-protected-package-private-and-private-in)

|Modifier|Class|Package|Subclass(same pkg)|Subclass(diff pkg)|World|
|---|---|---|---|---|---|
|public|Y|Y|Y|Y|Y|
|protected|Y|Y|Y|Y|N|
|*no modifier*|Y|Y|Y|N|N|
|private|Y|N|N|N|N|

* [static 클래스의 쓰임새](https://stackoverflow.com/questions/7486012/static-classes-in-java)
  * [Ex: Math class의 PI, E](https://hg.openjdk.java.net/jdk/jdk11/file/1ddf9a99e4ad/src/java.base/share/classes/java/lang/Math.java)
  ```
  // import java.lang.Math;
  public static final double E = 2.718281828459045;
  public static final double PI = 3.141592653589793;
  ```

* [Java의 main 메소드의 의미(public, static)](https://stackoverflow.com/questions/52803874/please-explain-every-element-of-java-main-public-static-void-mainstring-arg)
```
public : 콘솔에서 접근할 수 있게
static : 프로그램 실행시 바로 메모리에 할당하기 위해서
void : 반환값이 없는
main : main 이름
```

* String 클래스를 이용해서 문자열 결합을 할 때 문자열 인스턴스가 계속해서 생겨나는 것은 바람직한 현상이 아니다! 따라서 이 경우에는 문자열 인스턴스 생성을 최소화해가며 문자열을 결합할 수 있도록 StringBuilder 클래스를 사용하는 것이 좋다!

* [StringBuffer와 StringBuilder의 차이
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
기본적으로 속도의 차이가 있고, 스레드에서 돌아가는가 아닌가의 차이가 있다.
1149
84
```

* [@Override 어노테이션](https://velog.io/@pearl0725/Override-%EC%96%B4%EB%85%B8%ED%85%8C%EC%9D%B4%EC%85%98%EC%9D%98-%EC%9D%98%EB%AF%B8%EC%99%80-%EC%82%AC%EC%9A%A9-%EC%9D%B4%EC%9C%A0%EB%8A%94-%EB%AC%B4%EC%97%87%EC%9D%BC%EA%B9%8C)

* [int[] array와 int array[]의 차이](https://stackoverflow.com/questions/129178/difference-between-int-array-and-int-array)
```
int[] foo, bar; // foo, bar = array
int foo[], bar; // foo = array, bar = int
```

* [자주 헷갈릴 수 있는 것 : 오버로딩 vs 오버라이딩](https://stackoverflow.com/questions/154577/polymorphism-vs-overriding-vs-overloading)
```
오버로딩 : 매개변수가 다른 것
오버라이딩 : 부모클래스의 메소드와 같은 이름의 메소드를 재정의하여 쓰는 것
```

* [자바에서 super.super.method()가 허용 되지 않는 이유](https://stackoverflow.com/questions/586363/why-is-super-super-method-not-allowed-in-java)
```
캡슐화
```

* [abstract interface 쓰는 이유](https://stackoverflow.com/questions/7202616/java-abstract-interface)

* [interface 와 abstract class 의 차이](https://stackoverflow.com/questions/1913098/what-is-the-difference-between-an-interface-and-abstract-class/1913185#1913185)

* [메모리 영역 1](https://docs.oracle.com/javase/specs/jvms/se15/html/jvms-2.html#jvms-2.5.4)

* [메모리 영역 2](https://stackoverflow.com/questions/79923/what-and-where-are-the-stack-and-heap?page=1&tab=scoredesc#tab-top)

## Web 북마크
* [html, css cheatsheet](https://docs.emmet.io/cheat-sheet/)

* [웹 기초](https://w3schools.com/)

* [Mozilla Developer Network](https://developer.mozilla.org/ko/)

## PS/CP
* [Tip](https://cses.fi/book/book.pdf)
* [ㅇㅇ](https://drive.google.com/file/d/1J2x8pIYQ3MXANgvzOgBciWd3d79j_Exa/view)
* [USACO GUIDE](https://usaco.guide/)
* [댓글 참고](https://codeforces.com/blog/entry/85668)
