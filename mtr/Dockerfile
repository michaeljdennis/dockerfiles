# Usage: docker run --rm -it michaeljdennis/mtr google.com
#
FROM ubuntu:18.04

LABEL maintainer "Michael Dennis <michaeljdennis@gmail.com>"

RUN apt-get update \
    && apt-get install -y mtr \
    --no-install-recommends

ENTRYPOINT ["mtr"]
