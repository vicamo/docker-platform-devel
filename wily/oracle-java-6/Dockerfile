FROM vicamo/android-pdk:wily-oracle-java-6

RUN echo "deb http://archive.ubuntu.com/ubuntu wily main restricted universe multiverse" > /etc/apt/sources.list.d/archive.ubuntu.com_wily.list && \
	echo "deb-src http://archive.ubuntu.com/ubuntu wily main restricted universe multiverse" >> /etc/apt/sources.list.d/archive.ubuntu.com_wily.list && \
	echo "deb http://archive.ubuntu.com/ubuntu wily-updates main restricted universe multiverse" >> /etc/apt/sources.list.d/archive.ubuntu.com_wily.list && \
	echo "deb-src http://archive.ubuntu.com/ubuntu wily-updates main restricted universe multiverse" >> /etc/apt/sources.list.d/archive.ubuntu.com_wily.list && \
	echo "deb http://archive.ubuntu.com/ubuntu wily-security main restricted universe multiverse" >> /etc/apt/sources.list.d/archive.ubuntu.com_wily.list && \
	echo "deb-src http://archive.ubuntu.com/ubuntu wily-security main restricted universe multiverse" >> /etc/apt/sources.list.d/archive.ubuntu.com_wily.list && \
	echo "deb http://ppa.launchpad.net/phablet-team/tools/ubuntu wily main" > /etc/apt/sources.list.d/ppa.launchpad.net_phablet-team_wily.list && \
	cat /dev/null > /etc/apt/sources.list && \
	apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 5C5364B55E51A24C && \
	apt-key adv --keyserver keyserver.ubuntu.com --recv-keys C2518248EEA14886 && \
	apt-get update && \
	apt-get install --no-install-recommends -y \
		abootimg \
		cpio \
		g++-4.8-multilib \
		imagemagick \
		kmod \
		libasound2-dev:i386 \
		libesd0-dev:i386 \
		libpulse-dev:i386 \
		openssh-client \
		phablet-tools \
		pxz \
		ubuntu-device-flash \
		ubuntu-emulator \
		&& \
	apt-get clean && \
	rm -f /var/lib/apt/lists/*_dists_*
