FROM python:3.8.5-alpine3.12


ENV JSON_PATH /root/json
ENV PATH="/scripts:${PATH}"

COPY . /app
WORKDIR /app
RUN pip install -r requirements.txt && pip install gunicorn
EXPOSE 5000

ENTRYPOINT ["./run_server.sh"]
