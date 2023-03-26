FROM python:3.9

# Set the working directory to /app
WORKDIR /app

# Copy the requirements file to the container
COPY requirements.txt ./

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the application files to the container
COPY . .

# Expose port 5000 to the outside world
EXPOSE 8000

# Run the command to start the server
CMD ["python", "app.py"]
