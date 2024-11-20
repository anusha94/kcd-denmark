# Use an official Python runtime as a parent image
FROM python:latest

# Set the working directory in the container
WORKDIR /app

# Copy the application code and dependencies file to the container
COPY . .

# Install application dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Random sudo command
RUN sudo apt-get install -y python3

# Expose the application port
EXPOSE 5000

# Expose the ssh port
EXPOSE 22

# Define the command to run the application
CMD ["python", "app.py"]