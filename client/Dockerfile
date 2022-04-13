FROM node:alpine
 
# Add the following line 
ENV CI=true
 
WORKDIR /app
COPY package.json ./
RUN npm config set legacy-peer-deps true
RUN npm install
COPY ./ ./
 
CMD ["npm", "start"]