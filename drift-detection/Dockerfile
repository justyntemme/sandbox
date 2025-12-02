# Use a lightweight base image
FROM python:3.9-slim

# Set working directory
WORKDIR /app

# Create a harmless dummy file to serve
RUN echo "<html><body><h1>Prisma Cloud Drift Demo</h1></body></html>" > index.html

# Create a specific folder we can 'drift' later
RUN mkdir /app/safe_folder

# Expose port 8000
EXPOSE 8000

# Run a simple HTTP server to keep the container alive and listening
CMD ["python", "-m", "http.server", "8000"]
