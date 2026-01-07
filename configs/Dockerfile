FROM clickhouse/clickhouse-server:25.3
# RUN yum install -y unixODBC  # драйверы ODBC если нужны
USER root
RUN mkdir -p /docker-entrypoint-initdb.d
COPY init.sql /docker-entrypoint-initdb.d/
USER clickhouse
