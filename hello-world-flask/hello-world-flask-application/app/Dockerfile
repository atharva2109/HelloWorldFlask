FROM tiangolo/meinheld-gunicorn-flask:python3.8
ENV LISTEN_PORT=5000
EXPOSE 5000

WORKDIR /app

COPY ./requirements.txt ./requirements.txt
RUN pip3 install -r ./requirements.txt

COPY . .

ENTRYPOINT [ "python" ]

CMD ["main.py" ]