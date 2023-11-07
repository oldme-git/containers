# oldme-git/alpine:3.18
FROM alpine:3.18

LABEL maintainer="tyyn1022@gmail.com"

# 使用阿里alpine源
RUN echo http://mirrors.aliyun.com/alpine/v3.18/main/ > /etc/apk/repositories \ 
	&& apk update && apk add tzdata ca-certificates bash \
	&& rm -rf /etc/localtime && cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
	&& echo "Asia/Shanghai" > /etc/timezone