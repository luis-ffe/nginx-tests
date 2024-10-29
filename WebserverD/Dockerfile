# Use the official Nginx image as the base
FROM nginx:latest

# Copy configuration files
#COPY conf/default.conf /etc/nginx/conf.d/default.conf
COPY nginx.conf /etc/nginx/nginx.conf

# Copy website and error pages
COPY homepage /usr/share/nginx/html/homepage
COPY errors /usr/share/nginx/html/errors

# Expose port 80
EXPOSE 80

# Start Nginx in the foreground
CMD ["nginx", "-g", "daemon off;"]
