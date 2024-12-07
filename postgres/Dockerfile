FROM postgres:15

# Copy any initialization scripts if needed
COPY *.sql /docker-entrypoint-initdb.d/

# Expose the PostgreSQL port
EXPOSE 5432