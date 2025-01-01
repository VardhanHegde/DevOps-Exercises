# Use the official Python image as the base image
FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /app

# Copy the Python script to the container
COPY delivery_metrics.py .

# Install necessary Python dependencies
RUN pip install prometheus_client

# Expose the port for the metrics endpoint
EXPOSE 8000

# Run the Python script
CMD ["python", "delivery_metrics.py"]
