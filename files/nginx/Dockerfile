FROM nginx:1.7
LABEL maintainer="aisna@protonmail.com"


# set timezome
ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
#
# Install package and PHP Core extensions
RUN apt-get update && apt-get install -y \
        git lsof htop vim subversion
