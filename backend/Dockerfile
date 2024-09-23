FROM directus/directus:11.1.0

# Switch to root user to install packages
USER root

# Install Git using apk
RUN apk update && \
    apk add git

# Switch back to the 'node' user for safety
USER node

USER root
RUN corepack enable
USER node
