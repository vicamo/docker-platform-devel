FROM vicamo/platform-devel-base:vivid-oracle-java-6

RUN echo "deb http://archive.ubuntu.com/ubuntu/ utopic universe" > /etc/apt/sources.list.d/utopic-mingw32.list \
	&& apt-get update \
	&& apt-get install --no-install-recommends -y \
		bc \
		lzop \
		mingw32 \
		tofrodos \
	&& apt-get clean \
	&& rm -f /var/lib/apt/lists/*_dists_*
