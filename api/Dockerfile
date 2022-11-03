FROM python:3.7.3-stretch

# Create a working directory
WORKDIR /app

# Copy source code to working directory
COPY ./requirements.txt /app/requirements.txt

# Install packages from requirements.txt
RUN pip install --no-cache-dir -r /app/requirements.txt

# Copy source code to working directory
COPY ./api /app/api
COPY ./manage.py /app/manage.py

# Run manage.py at container launch
CMD ["python", "manage.py", "runserver"]