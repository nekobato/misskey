FROM node:22.23.5-bookworm@sha256:e13726ca604184d7a91fcacab1fc09eefd642dc28e79ac34e85540dd93b78cfb

RUN apt-get update \
	&& apt-get install -y --no-install-recommends sudo \
	&& echo 'node ALL=(root) NOPASSWD:ALL' > /etc/sudoers.d/node \
	&& chmod 0440 /etc/sudoers.d/node \
	&& corepack enable \
	&& rm -rf /var/lib/apt/lists/*
