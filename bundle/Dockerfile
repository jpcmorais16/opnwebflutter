FROM cirrusci/flutter

RUN useradd -ms /bin/bash developer
USER developer
WORKDIR /home/developer
COPY ["opn_flutter", "/home/developer/"] 
COPY ["lib", "/home/developer/lib/"]
COPY ["data", "/home/developer/data/"]

EXPOSE 80

ENTRYPOINT [ "/home/developer/opn_flutter" ]