FROM python:3.11-slim

# Defined the working directory
WORKDIR /app

# Install all the dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy the files
COPY . .

#EXPOSE port 80
EXPOSE 80

# Start App
CMD ["python", "app.py"]
