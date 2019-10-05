FROM alpine:3.8

LABEL maintainer "Michael Dennis <michaeljdennis@gmail.com>"

ARG AWS_DEFAULT_REGION
ARG AWS_ACCESS_KEY_ID
ARG AWS_SECRET_ACCESS_KEY

RUN apk add --no-cache python3 \
    py-pip \
    && pip3 install awscli \
    && mkdir -p /root/.aws \
    && { \
		echo '[default]'; \
		echo "region = $AWS_DEFAULT_REGION"; \
	} > /root/.aws/config \
    && { \
		echo '[default]'; \
		echo "aws_access_key_id = $AWS_ACCESS_KEY_ID"; \
		echo "aws_secret_access_key = $AWS_SECRET_ACCESS_KEY"; \
	} > /root/.aws/credentials

ENTRYPOINT ["sh"]
