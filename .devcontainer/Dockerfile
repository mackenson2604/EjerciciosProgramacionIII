FROM node:22-slim

USER root

# Configurar mirror de Debian alternativo (Aliyun - HTTP)
RUN sed -i 's|http://deb.debian.org/debian|http://mirrors.aliyun.com/debian|g' /etc/apt/sources.list.d/debian.sources

# Actualizar e instalar dependencias
RUN apt-get update -qq && \
    apt-get install -y --no-install-recommends curl ca-certificates && \
    rm -rf /var/lib/apt/lists/*

USER node