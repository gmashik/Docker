FROM python:3.7.3-slim
LABEL maintainer="G M Ashikur Rahman (gmarahma@uwaterloo.ca)"
LABEL version="1.0"
LABEL description="Noteboook and data (.csv file) to build a machine learning 
                     model for spam filter application"

WORKDIR /data

COPY . /data

RUN pip install numpy pandas sklearn matplotlib nltk seaborn jupyter

EXPOSE 8888

CMD ["jupyter","notebook","--ip=0.0.0.0", "--port=8888", "--no-browser", "--allow-root"]
