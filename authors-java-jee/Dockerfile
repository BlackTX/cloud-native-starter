FROM open-liberty:19.0.0.9-kernel-java11

COPY liberty/server.xml /config/

COPY target/authors.war /config/apps/

# This script will add the requested XML snippets, grow image to be fit-for-purpose and apply interim fixes
# https://github.com/WASdev/ci.docker
RUN configure.sh

EXPOSE 3000
