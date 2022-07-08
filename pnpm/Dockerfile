FROM node:16-alpine

# Add curl + libc6-compat
# Check https://github.com/nodejs/docker-node/tree/b4117f9333da4138b03a546ec926ef50a31506c3#nodealpine to understand why libc6-compat might be needed.
RUN apk --no-cache add \
    curl \
    libc6-compat

# Add pnpm
RUN curl -sL https://unpkg.com/@pnpm/self-installer | node