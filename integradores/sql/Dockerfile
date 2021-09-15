# mssql-server-linux
# Maintainers: Microsoft Corporation (LuisBosquez and twright-msft on GitHub)
# GitRepo: https://github.com/Microsoft/mssql-docker

# Base OS layer: Latest Ubuntu LTS.
FROM ubuntu:16.04

# Default SQL Server TCP/Port.
EXPOSE 1433

# Copy all SQL Server runtime files from build drop into image.
ENV MSSQL_COLLATION= "SQL_Latin1_General_CP850_CI_AI"
ENV SQLCOLLATION="SQL_Latin1_General_CP850_CI_AI"

COPY ./install /

# Run SQL Server process.
CMD [ "/opt/mssql/bin/sqlservr" ]


