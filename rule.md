


## 네이밍 규칙


**함수 네이밍**
```c
ex)
1. 항상 기능 목적의 동사가 앞에 오도록 한다.
validate_input(int argc);
```

```c
2. get, set 함수를 이용해 값을 가져오거나 설정하는 것을 최우선적으로 사용한다.
get_input(int argc);
set_input(int argc);

3. init_ 종류의 함수는 초기화를 목적으로 하는 상황에서 사용한다.
init_input(int argc);

```

**파일 구조**

3. 한 개의 파일은 하나의 기능만 하는 함수를 담는다.
만약 함수에서 다른 함수가 필요하게 된다면, 코드 최상단에 선언한다.

3-1. 만약 함수에서 사용해야하는 함수가 다중으로 필요하다면 새로운 파일로 분리하여 사용한다.

**변수명 규칙**

4. 반복문은 i변수를 활용하고, 배열을 핸들링 하기 위한 변수는 idx로 사용한다.
4-1. 숫자 및 갯수는 ```nbr```로 사용한다.
4-2.복수 및 단수의 구분도 확실하게 해준다. 단수 :```input```  복수 :```inputs ```

**중괄호 규칙**
아래와 같이 생략이 가능한 상황이라면 중괄호의 생략을 허용한다.
```c
if(true)
	printf("hello world"); 
```