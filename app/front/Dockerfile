FROM nginx:alpine

WORKDIR /app
COPY . .

# Set the environment variable
ENV WS_BACK_URL=http://localhost:5000

RUN chmod +x ./entrypoint.sh

# Lancer Nginx en mode foreground
CMD ["nginx", "-g", "daemon off;"]