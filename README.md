# InstaClone

InstagramClone including auth, posts, comments, tags, direct messages and notifications

## Screenshots
![Alt text](/screenshots/login.png?raw=true "Login")
![Alt text](/screenshots/index.png?raw=true "Index")
![Alt text](/screenshots/index-dark.png?raw=true "Index-Dark")
![Alt text](/screenshots/post.png?raw=true "Post")
![Alt text](/screenshots/profile.png?raw=true "Profile")
![Alt text](/screenshots/dms.png?raw=true "Direct Messages")

## Setup
- ``` git clone https://github.com/kurekhombre/InstaClone.git ```
- Create virtual environment ```python3 -m venv venv``` and activate it
  - Linux/Mac ``` source venv/bin/activate ```
  - Windows ``` venv\Scripts\activate.bat ```
- ``` pip install -r requirements.text ```
- Generate SECRET KEY with 
  - https://djecrety.ir/ or 
  - ``` python manage.py shell ``` 
   ``` >>> from django.core.management.utils import get_random_secret_key``` 
  ``` print(get_random_secret_key) ```
- Create  file '.env' in project folder and paste ``` SECRET_KEY='<your_key>' ```
- ``` python manage.py makemigrations ```
- ``` python manage.py migrate ```
- ``` python manage.py runserver ```


## Issues / TODO
1. Notifications Problem
2. PostgreSQL database instead of sqlite
3. Direct Messages Frontend
4. DM with WebSockets (Django Channels + Redis)
5. Stories logic
6. 1/2 images are not displaying correctly
7. Google, Facebook auth todo
8. Email token (register/reset password)
9. Edit profile (remove required fields and avatar upload issue)
10. Black theme works only in index.html
11. Messages are duplicated
