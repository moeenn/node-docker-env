FROM node:16-alpine

WORKDIR /app

COPY ./backend/entrypoint.sh /entrypoint.sh
RUN chmod +x /entrypoint.sh

ENTRYPOINT ["/bin/sh", "/entrypoint.sh"]
RUN npm i --global npm
CMD ["npm", "run", "dev"]

EXPOSE 5000