ARG VERSION
FROM redis:${VERSION}

LABEL maintainer="ChanYu"

# 复制时区配置
ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

CMD [ "redis-server"]

EXPOSE 6379
