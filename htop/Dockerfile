# htop in a container

# docker run --rm -it \
# 	--pid host \
# 	diggajupadhyay/htop
#
FROM alpine:latest
LABEL maintainer "Diggaj Upadhyay"

RUN apk --no-cache add \
	htop

CMD [ "htop" ]
