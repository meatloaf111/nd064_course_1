FROM python:3.8


WORKDIR /app
COPY techtrends ./

RUN pip install -r requirements.txt

RUN python init_db.py

ENV PORT 3111
EXPOSE ${PORT}

CMD [ "python", "app.py"]