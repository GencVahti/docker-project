FROM python:3.8-slim
WORKDIR /app
COPY dependencies.txt .
RUN pip install -r dependencies.txt
COPY src/ .
# COPY . .
EXPOSE 5001
CMD ["python", "./server.py"]