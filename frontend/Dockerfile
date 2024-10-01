# Stage 1: Build Angular App
FROM node:14 AS node-build

# Set working directory inside the container
WORKDIR /app

# Copy all project files to the container
COPY . /app

# Install dependencies
RUN npm install

# Build the Angular app for production
RUN npm run build --prod

# Stage 2: Run Angular App with Node.js
FROM node:14

# Set working directory
WORKDIR /app

# Copy the build output from the previous stage
COPY --from=node-build /app /app

# # Expose the port that Angular uses (default 4200)
# EXPOSE 4200

# # Start the Angular app
# CMD ["npm", "start"]

# Stage 2: Serve the app with nginx
FROM nginx:alpine

# Copy the build output to the nginx html directory
COPY --from=node-build /app/dist/frontend /usr/share/nginx/html
COPY nginx.conf /etc/nginx/nginx.conf

