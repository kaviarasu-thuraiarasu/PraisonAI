FROM python:3.11-slim
WORKDIR /app
COPY . .
RUN pip install flask praisonai==2.2.18 gunicorn markdown
EXPOSE 8080
CMD ["gunicorn", "-b", "0.0.0.0:8080", "api:app"]
