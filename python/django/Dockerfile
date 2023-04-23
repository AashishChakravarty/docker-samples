# Start with an official Python runtime as a parent image
FROM python:3.9-slim-buster

# Set the working directory for the Docker container
WORKDIR /app

# Copy the requirements.txt file to the container
COPY requirements.txt .

# Install the dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the application files to the container
COPY . .

# Expose the port that the Django application will run on
EXPOSE 8000

# Run the Django application with gunicorn
CMD ["gunicorn", "--bind", "0.0.0.0:8000", "myapp.wsgi:application"]