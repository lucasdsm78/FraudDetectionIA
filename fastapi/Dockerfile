FROM python:3.9-slim

WORKDIR /app

COPY . .

# Install FastAPI dependencies
RUN pip install --trusted-host pypi.python.org -r requirements.txt

# Make port 80 available to the world outside this container
EXPOSE 8000

# Run FastAPI when the container launches
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]