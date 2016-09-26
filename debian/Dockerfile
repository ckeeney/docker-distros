FROM debian
# Todo: it should be possible to just submodule github.com/docker/docker and build this entire image more cleanly using build scripts

# remove the docker setups from apt.  this has a considerable impact on docker image size.
RUN rm -f /etc/apt/apt.conf.d/docker-*

# ensure all packages listed by 'dpkg --get-selections | grep -v deinstall' of a fresh debian are installed
RUN (DEBIAN_FRONTEND=noninteractive; apt-get update && apt-get install -y python cron

CMD ["/bin/bash"]
