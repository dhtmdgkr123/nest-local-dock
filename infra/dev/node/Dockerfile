ARG nodeVersion=lts
FROM node:${nodeVersion}

LABEL maintainer="dhtmdgkr123<osh12201@gmail.com>"

ARG codePathContainer=/app
RUN mkdir -p ${codePathContainer}
WORKDIR ${codePathContainer}

COPY . ${codePathContainer}
COPY ./aliases.sh /root/aliases.sh
COPY ./aliases.sh /root/aliases.sh

RUN \
    ########## install nest cli ##########
    npm install -g @nestjs/cli && \
    ########## install nest cli ##########
    ########## load custom alias ##########
    sed -i 's/\r//' /root/aliases.sh && \
    echo "" >> ~/.bashrc && \
    echo "# Load Aliases" >> ~/.bashrc && \
    echo "source ~/aliases.sh" >> ~/.bashrc && \
    echo "" >> ~/.bashrc
    ########## load custom alias ##########
    
ENTRYPOINT ["npm", "run", "start:dev"]