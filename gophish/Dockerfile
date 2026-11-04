# Imagen base de GoPhish con versión fija
FROM gophish/gophish:0.12.1

# Usuario administrador para preparar los directorios
USER root

# Crear el directorio de persistencia de SQLite
# y asignar permisos al usuario de la aplicación
RUN mkdir -p /opt/gophish/data \
    && chown -R app:app /opt/gophish/data

# Ejecutar GoPhish sin privilegios de administrador
USER app
