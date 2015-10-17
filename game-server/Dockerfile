FROM ubuntu:14.04

RUN set -x \
        && apt-get update \
        && apt-get install -y --no-install-recommends \
            curl \
            postgresql-9.3
RUN curl http://pwnadventure.com/PwnAdventure3Server.tar.gz -o /tmp/PwnAdventure3Server.tar.gz

RUN mkdir -p /opt/pwn-adventure3 \
        && tar -x -z -v -f /tmp/PwnAdventure3Server.tar.gz --strip-components=1 -C /opt/pwn-adventure3 \
        && rm /tmp/PwnAdventure3Server.tar.gz
