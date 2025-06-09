FROM python:3.12.10-alpine
LABEL maintainer="@uday"

COPY /${{ values.app_name }}/requirements.txt /tmp

RUN pip install -r /tmp/requirements.txt

COPY ./${{ values.app_name }} /${{ values.app_name }}

CMD python /${{ values.app_name }}/app.py
