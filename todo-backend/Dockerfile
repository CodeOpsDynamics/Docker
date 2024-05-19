FROM python:alpine3.19
WORKDIR /app
#WORKDIR helps in running cd and mkdir
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . .
#RUN pip install -r requirements.txt
ENV MYSQL_USER=root
ENV MYSQL_PASSWORD=my_password
ENV MYSQL_DATABASE=my_database
CMD ["flask", "run", "--host=0.0.0.0", "--port=8000"]

#docker run --name mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=my_password -e MYSQL_DATABASE=my_database -d mysql
# -p is for ports , -e for env variables, --name mysql(nick name not neccessary)