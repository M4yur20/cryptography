# FROM python:3
#
# ENV PYTHONUNBUFFERED 1
#
# WORKDIR /app
#
# ADD . /app
#
# COPY ./requirements.txt /app/requirements.txt
#
# RUN pip install -r requirements.txt
#
# RUN python manage.py makemigrations
#
# RUN python manage.py migrate
#
# COPY . /app


FROM python:3.6
ENV PYTHONUNBUFFERED 1
RUN mkdir /my_app_dir
WORKDIR /my_app_dir
ADD requirements.txt /my_app_dir/
RUN pip install --upgrade pip && pip install -r requirements.txt
ADD . /my_app_dir/