django 초기 설정 명령어

# 가상 환경 생성
python -m venv venv 
# 가상환경 활성화(mac)
source venv/bin/activate
# 가상환경 활성화(window)
source venv/Scripts/activate
# django 설치
pip install django
# 가상 환경 종료
deactivate

# 패키지 목록 확인
pip list
# 의존성 기록
pip freeze > requirements.txt
# 의존성 설치
pip install -r requirements.txt

# 만들기
django-admin startproject pjt .
# articles 만들기
python manage.py startapp articles
# 서버 실행
python manage.py runserver


# 모델 변경 사항을 감지해서 migration 파일 생성-설계도
python manage.py makemigrations
# 데이터베이스에 적용-설계도 반영
python manage.py migrate
# 슈퍼유저 생성
python manage.py createsuperuser

# ipython 설치
pip install ipython
# django-extensions 설치
pip install django-extensions
# Django Shell에 접속하기
python manage.py shell
# 강제로 하믄 되듯이 이것씀
python manage.py shell_plus
# Django Shell에서 나가고 싶을때
exit()
# shell-v 옵션
python manage.py shell -v2