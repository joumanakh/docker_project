FROM ultralytics/yolov5:latest-cpu
WORKDIR /usr/src/app
RUN pip install --upgrade pip
COPY requirements.txt .
RUN pip install -r requirements.txt
RUN curl -L https://github.com/ultralytics/yolov5/releases/download/v6.1/yolov5>

COPY . .
#********
# Install boto3
RUN pip install boto3
# Install additional dependencies
RUN pip install pymongo
#********
CMD ["python3", "app.py"]

