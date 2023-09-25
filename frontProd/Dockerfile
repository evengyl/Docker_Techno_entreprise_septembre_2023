FROM node:lts-slim as builder

WORKDIR /app

COPY . .

FROM nginx:stable-alpine3.17-slim

COPY --from=builder /app/* /usr/share/nginx/html/

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]