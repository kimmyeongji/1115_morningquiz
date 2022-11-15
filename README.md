# 1115_morningquiz

1. 아래의 코드를 다운로드 받으세요.

[ai2_back.zip](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1bb7200d-c645-4d2b-95dc-5b73f7fd5fe5/ai2_back.zip)

2. 가상환경을 설정 해주세요.
    
    `python3 -m venv myvenv`
    
    `source myvenv/bin/activate`
    
    `pip install -r requirements.txt`
    

3. 본 프로젝트의 user.views.UserView.as_view()를 호출하면 아래와 같은 응답을 받게 됩니다.
    
    ```jsx
    {'message': '가입 완료!!'}
    ```
    

user app의 **test.py**에 테스트 클래스 및 메서드를 적절히 작성하여

올바르게 회원가입이 완료되었을 때 “가입 완료!!”라는 문자열이 제대로 뜨는지 확인하는 테스트를 작성하여

깃허브에 push 한 뒤 링크를 제출해주세요.

조건1.  rest_framework.test의 APITestCase 를 사용하세요.

조건2. response의 status code가 200인지를 검사하는 문항이 **아니라** 

     응답의 message가 '가입 완료!!' 라는 문자열과 동일한지를 검사하는 테스트를 만드세요.

     다시 말해 아래의 코드는 오답입니다.

```jsx
self.assertEqual(response.status_code, 200)
```

올바르게 작성한 경우 python [manage.py](http://manage.py) test 명령어 입력시 아래와 같이 나오게 됩니다.
