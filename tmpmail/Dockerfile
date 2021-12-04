FROM alpine

RUN apk add --no-cache curl jq w3m

RUN curl -L "https://git.io/tmpmail" > tmpmail && chmod +x tmpmail

RUN mv tmpmail /bin/
