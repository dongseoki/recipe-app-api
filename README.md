# recipe-app-api
Recipe API project

* [Build a Backend REST API with Python & Django - Advanced](https://www.udemy.com/course/django-python-advanced/)를 들으면서 따라한 클론 코딩.

* Python 과 Django, Django rest framework을 이용해 recipe서비스에 필요한 API를 따라서 만들어보는 강의
* 아래에 해당하는 것들을 배움.
    * docker 기반의 격리된 환경구성
    * TDD 기반의 개발 방법
    * Django rest framework 활용법
    * Swagger를 이용한 API 명세서 작성 방법을 익힘.

# 프로젝트를 로컬에서 실행하는 방법.
```
git clone https://github.com/dongseoki/recipe-app-api.git
cd recipe-app-api
docker-compose build
docker-compose up
```
* 이후 아래 url에서 Swagger를 이용한 API 명세 확인 및 API 테스트가 가능.
* http://127.0.0.1:8000/api/docs

# 프로젝트의 테스트코드 정상 동작 유무를 확인하는 방법
* 로컬 실행 설정 완료후
```
cd recipe-app-api
docker-compose run --rm app sh -c "python manage.py test"
```