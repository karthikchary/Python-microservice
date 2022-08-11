FROM python:3.9
RUN pip3 install --upgrade pip
RUN adduser karthik
USER karthik
WORKDIR /app
COPY --chown=karthik:karthik requirements.txt /app/requirements.txt
RUN pip install --user -r requirements.txt
COPY . /app

CMD python manage.py runserver 0.0.0.0:8000
