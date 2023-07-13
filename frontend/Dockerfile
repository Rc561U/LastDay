FROM node:18.12.0-buster

ENV TZ Asia/Tokyo
# Create a non-root user
RUN addgroup --system myuser && adduser --system --ingroup myuser myuser

# Set the user as the default user
USER myuser

WORKDIR /src

RUN yarn global add @vue/cli
EXPOSE 3000
ENTRYPOINT ["yarn", "dev"]