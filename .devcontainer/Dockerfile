FROM node:22.23.4-bookworm@sha256:2bd396628eceb5c999a6e43731fab69d5fb98b94ba9d9d90b5f64575c5178765

RUN apt-get update \
	&& apt-get install -y --no-install-recommends sudo \
	&& echo 'node ALL=(root) NOPASSWD:ALL' > /etc/sudoers.d/node \
	&& chmod 0440 /etc/sudoers.d/node \
	&& corepack enable \
	&& rm -rf /var/lib/apt/lists/*
