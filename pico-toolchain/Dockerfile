# https://rptl.io/pico-get-started

FROM debian

# Install the Toolchain
RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get install -y \
  cmake \
  gcc-arm-none-eabi \
  libnewlib-arm-none-eabi \
  build-essential \
  python3

RUN apt-get clean && rm -rf /var/lib/apt/lists/*

WORKDIR "/root"
CMD [ "/bin/bash" ]
