# Use the official Nginx image from Docker Hub
FROM nginx:latest

# Copy custom HTML file to serve as a web page
COPY index.html /usr/share/nginx/html/index.html

# Expose port 80 to allow external access
EXPOSE 80

# Start Nginx when the container starts
CMD ["nginx", "-g", "daemon off;"]
