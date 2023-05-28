FROM s390x/ubuntu:20.04

WORKDIR .

RUN apt-get update && apt-get install -y \
    build-essential \
    make \
    cmake \



COPY . .

RUN ./test/travis_run_linux.sh

CMD ["echo", "Build is success"]
