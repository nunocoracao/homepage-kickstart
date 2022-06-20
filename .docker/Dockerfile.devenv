# Start with Hugo Docker image
FROM klakegg/hugo:0.93.2-ubuntu

# Download Curl, Node, NPM, and Firebase
RUN apt-get -y update && apt-get -y upgrade && \
    apt-get install -y curl nodejs npm && \
    npm install -g firebase-tools

# Hugo dev server port
EXPOSE 1313