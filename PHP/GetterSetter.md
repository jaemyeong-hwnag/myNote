# GetterSetter

## GetterSetter는 PHP에 필요한가?

목차
> [1. 구글](#1.-구글) <br>
> [2. stackoverflow](#2.-stackoverflow)

## 1. 구글
> PHP로 클래스를 작성할 때 순진한 setter 및 getter를 작성하는 대신 객체 속성을 직접 사용하여, <br> 
> 시간을 절약하고 스크립트 속도를 높일 수 있습니다.

> 아래 코드의 1번 예시 보다 2번 예시가 개발 시간을 단축 할뿐만 아니라, <br>
> 최대 100% 더 빠르게 실행할 수 있다고 한다.

> 아래
<pre>
  <code>
    class dog {
      public $name = '';

      public function setName($name) {
       $this->name = $name;
      }

      public function getName() {
       return $this->name;
      }
    }
  </code>
</pre>


> 예시 1
> 
  <pre>
    <code>
      $rover = new dog();
      $rover->setName('rover');
      echo $rover->getName();
    </code>
  </pre>
> 예시 2
> 
  <pre>
    <code>
      $rover = new dog();
      $rover->name = 'rover';
      echo $rover->name;
    </code>
  </pre>
  
## 2. stackoverflow

> ### 답변 중

>> PHP는 Java, C ++ 또는 C #이 아닙니다. PHP는 다르며 역할도 다릅니다. <br>
>>> 1. 디버그하기가 어렵습니다. <br>
>>> 2. 성능에 부정적인 영향이 있습니다. <br>
>>> 3. 더 많은 코드를 작성해야합니다. <br>

## 출처
구글 - https://web.archive.org/web/20140625191431/https://developers.google.com/speed/articles/optimizing-php
stackoverflow - https://stackoverflow.com/questions/4478661/getter-and-setter
