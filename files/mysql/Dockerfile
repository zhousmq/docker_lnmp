FROM mysql:5.7
LABEL maintainer="aisna@protonmail.com"

# set timezome
ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
RUN apt-get update && apt-get install -y \
        git lsof htop vim subversion

# mysql backup scripts using crontab
# COPY ./scripts/ /data/mysql/backup/scripts/
# RUN crontab /data/mysql/backup/scripts/crontabfile
# RUN service cron start
