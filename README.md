# Image to PDF Converter

## Build Docker Image
To build the Docker image, run:

```bash
docker build -t image-to-pdf .

docker run --rm \
-v $(pwd)/images:/app/images \
-v $(pwd)/output:/app/output \
-e PDF_NAME=my_custom_output \
image-to-pdf /app/images
