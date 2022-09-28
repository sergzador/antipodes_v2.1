FROM mcr.microsoft.com/mssql/server:2019-CU15-ubuntu-20.04

USER root
RUN mkdir -p /usr/src/scripts
WORKDIR /usr/src/scripts 

COPY create-from-mdf.sql /usr/src/scripts 
COPY create-from-sql.sql /usr/src/scripts 
COPY entrypoint.sh /usr/src/scripts 

RUN chmod +x /usr/src/scripts/import-data.sh

USER mssql
ENTRYPOINT /bin/bash ./entrypoint.sh


