FROM python:3.11-slim
WORKDIR /app
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY src ./src
ENV PYTHONPATH=/app/src          # добавляем путь до пакета
ENTRYPOINT ["python","-m","detector"]  # теперь найдётся как src/detector