# Use an official Python runtime as a parent image
FROM python:3.9

# Set the working directory
WORKDIR /app

# Copy the requirements file and install dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the application code
COPY . .

# Set environment variables for Hugging Face and Transformers cache
ENV HF_HOME=/app/.cache/huggingface
ENV TOKENIZERS_PARALLELISM=false

# Ensure the cache directory exists and is writable
RUN mkdir -p /app/.cache/huggingface && chmod -R 777 /app/.cache

# Expose the port the app runs on
EXPOSE 7860

# Start the Flask/Gunicorn application
CMD ["gunicorn", "--timeout", "300", "-w", "2", "-b", "0.0.0.0:7860", "chatbot:app"]