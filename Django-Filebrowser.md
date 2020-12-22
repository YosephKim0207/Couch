#Django 웹프레임워크 구축하기

sudo apt install python3
sudo apt install python3-pip
sudo atp install python3-django

//가상화 내용 추가하기

Django-admin startproject {프로젝트명}

{프로젝트명} 디렉토리 내 manage.py가 있는 곳에서
python3 manage.py runserver


#filebrowser 어플리케이션 적용

Django-filebrowser : https://github.com/sehmaschine/django-filebrowser
Grappelli : https://github.com/sehmaschine/django-grappelli
Pillow : https://github.com/python-pillow/Pillow

python3 -m pip install --upgrade pip

pip3 install django-filebrowser
pip3 install Django-grappelli
python3 -m pip install --upgrade Pillow

생성된 Django 프로젝트 내 setting.py, urls.py 파일을 업로드 되어있는 settings.py, urls.py 파일로 교체

python3 manage.py collectstatic

python3 manage.py migrate

python3 manage.py createsuperuser
절차에 따라 suepruser 생성

python3 manage.py runserver로 테스트
(현재 버전에서는 ~/admin시 FileBrowser 보이지 않음! ~/admin/filebrowser/browse로 직접 접근 필요)
(해당 문제에 대한 QnA : https://github.com/sehmaschine/django-filebrowser/issues/365)


