#install Python
FROM python:3.11-slim

#Changes working directory
WORKDIR /app

#Copies .txt to /app & inastalls dependencies & remove .txt
COPY requirements.txt .
RUN pip install -r requirements.txt
RUN rm requirements.txt

#copies .py to /app
COPY app.py .

#Expose port
EXPOSE 5000

#Executes app.py
CMD ["python","app.py"]
