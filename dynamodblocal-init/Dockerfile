FROM ubuntu:18.04
#RUN apt-get update && apt-get install -y python3.7 && apt-get install -y wget && wget https://bootstrap.pypa.io/get-pip.py && python get-pip.py
RUN apt-get update && apt-get install -y python3.7 && apt-get install -y python3-pip
RUN pip3 install awscli --upgrade
COPY create-dynamodb-tables.sh .
COPY ftgo-order-history.json .
COPY wait-for-dynamodblocal.sh .

RUN ["chmod", "+x", "./wait-for-dynamodblocal.sh"]
RUN ["chmod", "+x", "./create-dynamodb-tables.sh"]

CMD ./wait-for-dynamodblocal.sh && ./create-dynamodb-tables.sh
