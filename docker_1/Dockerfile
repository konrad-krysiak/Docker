FROM ubuntu:20.04
MAINTAINER Konrad Krysiak

RUN apt-get update && \
	apt-get install -y openjdk-11-jdk curl unzip zip
RUN rm /bin/sh && ln -s /bin/bash /bin/sh
RUN curl -s "https://get.sdkman.io" | bash
RUN chmod a+x "$HOME/.sdkman/bin/sdkman-init.sh"
RUN source "$HOME/.sdkman/bin/sdkman-init.sh" && \
	sdk install kotlin && \
	sdk install gradle 7.2