#
# Chrome Dockerfile
#
# https://github.com/dockerfile/chrome
#

# Pull base image.
FROM ubuntu:20.04

# Install Chromium.
RUN apt-get update && \
  apt-get install -y \
  wget \
  dpkg \
  sudo &&\
  # sudo apt-get install libxss1 &&\
  cd /tmp \
  wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb \
  sudo dpkg -i google-chrome-stable_current_amd64.deb
# Define working directory.
WORKDIR /data

# Define default command.
CMD ["bash"]

# Expose ports.
EXPOSE 5901
