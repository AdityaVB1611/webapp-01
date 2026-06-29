# Use official lightweight Python image
FROM python:3.11-slim

# Set working directory
WORKDIR /app

# Copy requirements and install
COPY requirements.txt .
RUN pip install --no-cache-dir -r ./deployments/docker/requirements.txt

# Copy app source
COPY app.py .

# Expose port
EXPOSE 5000

# Run the app
CMD ["python", "app.py"]
