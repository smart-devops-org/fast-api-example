# Python 3.8을 기반으로 하는 이미지를 사용합니다.
FROM python:3.8-slim-buster

# 작업 디렉토리를 설정합니다.
WORKDIR /app

# 필요한 패키지를 설치합니다.
RUN apt-get update && apt-get install -y \
    gcc \
    && rm -rf /var/lib/apt/lists/*

# Python 의존성을 설치합니다.
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# 소스 코드를 복사합니다.
COPY ./ /app

# 애플리케이션을 실행합니다.
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "80"]