
FROM python:3.12-alpine

# Set the working directory inside the container
WORKDIR /app

# Install build dependencies
RUN apk add --no-cache gcc musl-dev linux-headers

# Copy the application code into the container
COPY app.py /app/

# Install Flask and netifaces
RUN pip install --no-cache-dir flask netifaces

# Expose the port that the app runs on
EXPOSE 8000

# Command to run the application
CMD ["python", "app.py"]
