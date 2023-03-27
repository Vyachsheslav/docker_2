
FROM python:3.10-alpine

RUN apk add git
RUN apk update
RUN git clone https://github.com/Vyachsheslav/crud_dz-6.git

RUN pip install -r /crud_dz-6/requirements.txt
EXPOSE 8000

CMD ["python", "/crud_dz-6/manage.py", "runserver", "0.0.0.0:8000", "--noreload"]