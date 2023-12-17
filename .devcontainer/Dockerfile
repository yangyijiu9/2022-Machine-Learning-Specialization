FROM python:3.8-slim

# 安装基本工具
RUN apt-get update && apt-get install -y \
    build-essential \
    git \
    curl \
    && rm -rf /var/lib/apt/lists/*

# 将 requirements.txt 复制到容器内
COPY requirements.txt /tmp/requirements.txt

# 安装 requirements.txt 中的 Python 依赖
RUN pip install --no-cache-dir -r /tmp/requirements.txt
