FROM python:3.8-slim
WORKDIR /app
COPY ../app.py /app
RUN pip install --no-cache-dir flask
EXPOSE 5000
ENV name=world
CMD ["python","app.py"]