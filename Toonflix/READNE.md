# 홈화면
![image](https://github.com/user-attachments/assets/05025ea8-c5b0-4f37-b638-c6c0a4c82057)


# 웹툰 정보 화면
![image](https://github.com/user-attachments/assets/ae092db3-5dbb-4516-88a5-748817056027)


### 배운점 
- Flutter가 widget을 빠르게 찾을 수 있게 widget에는 ID 같은 식별자 역할을 하는 key가 있다. 
- Scaffold는 screen을 위한 기본적인 레이아웃과 설정을 제공한다.
- await
    - awit 비동기 필드 내에서만 사용할 수 있다. async 붙은 곳
    - await는 해당 작업을 완료할 때 까지, 다른 작업을 하지 않는 다는 것, 즉 동기형식으로 작동
- setState( () {}) 쉽게 이해하기 -> 상태가 변했으니까 build 메소드를 다시 실행해!
- const는 컴파일 하기전에 값을 알고 있다는 것 

```
 FutureBuilder(
        future: webtoons,
        builder: (context, snapshot) { //snapshot은 Future의 상태!!
          if (snapshot.hasData) {
            return const Text('There is data!');
          }
          return const Text("Loding...");
        },
      ),
```
- clipBehavior는 자식의 부모 영역 침법을 제어 하는 방법
