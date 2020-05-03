FROM ubuntu:16.04

RUN apt-get update && apt-get install -y curl wget
COPY ./scriptfile.sh /
RUN chmod +x /scriptfile.sh
ENTRYPOINT ["/scriptfile.sh"]
CMD ["bin/bash", "./scriptfile.sh"]
