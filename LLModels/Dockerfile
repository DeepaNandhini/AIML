FROM python:latest

WORKDIR /app

COPY requirements.txt ./
COPY chatbot.py ./

RUN pip install --upgrade pip
RUN pip install -r requirements.txt

EXPOSE 8051
ENTRYPOINT ["streamlit","run","chatbot.py","--server.port=8501","--server.address=0.0.0.0"]