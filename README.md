# knote
Simple Spring Boot app to take notes

## Cambios realizados: soporte para MinIO

- Las imágenes de las notas se guardan en un servidor de objetos compatible con MinIO/S3 (cliente `io.minio:minio:6.0.8`), en lugar del disco local.
- Nota: las imágenes oficiales `minio/minio` fueron retiradas de Docker Hub y Quay.io, por lo que el servidor se ejecuta con `rustfs/rustfs`, compatible con la API de MinIO/S3. El código usa el cliente de MinIO sin cambios.
- Imagen Docker: https://hub.docker.com/r/pulgarinmajo/knote
