# Use official lightweight Python image
FROM python:3.11-slim

# Set working directory
WORKDIR /app

# Copy requirements and install
COPY deployments/docker/requirements.txt requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Copy app source
COPY deployments/docker/app.py .

# Expose port
EXPOSE 5000

# Run the app
CMD ["python", "app.py"]
