# URL: http://www.rollit5.link

## 서버 시작하기
```
$ git clone --recursive https://github.com/2022-Winter-Bootcamp-Team-K/docker.git
$ cd fronted
$ yarn 
```
## 환경변수
* backend/backend/.env
```
SECRET_KEY={DJANGO_SECERT_KEY}
DEBUG=TRUE
DATABASE_URL={DATABASE_URL}

AWS_ACCESS_KEY_ID={AWS_ACCESS_KEY_ID}
AWS_SECRET_ACCESS_KEY={AWS_SECRET_ACCESS_KEY}
AWS_REGION={AWS_REGION}
BUCKET_NAME={BUCKET_NAME}

EMAIL_ADDR={EMAIL_ADDR}
EMAIL_PASSWORD={EMAIL_PASSWORD}
```

* backend/db/db.env
```
MYSQL_DATABASE={DATABASE_NAME}
MYSQL_ROOT_USER={DATABASE_USER}
MYSQL_ROOT_PASSWORD={DATABASE_PASSWORD}
```
* frontend/.env
```
REACT_APP_BACKEND_URL={BACKEND_URL}
```
## 실행하기
```
$docker compose -f docker-compose.prod.yaml, docker-compose.elk.yaml up --build
```