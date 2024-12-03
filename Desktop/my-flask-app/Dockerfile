# Dockerfile
FROM python:3.9-slim

# Set working directory
WORKDIR /app

# Copy the requirements file
COPY requirements.txt /app/

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the application
COPY . /app/

# Expose the port Flask will run on
EXPOSE 5000

# Set the entry point to run the Flask app
CMD ["python", "app.py"]