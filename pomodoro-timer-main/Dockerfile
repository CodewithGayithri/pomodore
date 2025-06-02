# Use official Nginx image to serve static content
FROM nginx:alpine

# Set the working directory inside the container
WORKDIR /usr/share/nginx/html

# Remove default Nginx web files
RUN rm -rf ./*

# Copy all your frontend files into the container
COPY . .

# Expose port 80 for the container
EXPOSE 80

# Start Nginx when the container runs
CMD ["nginx", "-g", "daemon off;"]
