FROM node:16-alpine

WORKDIR /app

COPY ./frontend/entrypoint.sh /entrypoint.sh
RUN chmod +x /entrypoint.sh

ENTRYPOINT ["/bin/sh", "/entrypoint.sh"]
RUN npm i --global npm
CMD ["npm", "run", "dev"]

EXPOSE 3000