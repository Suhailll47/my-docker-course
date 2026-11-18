# Start from ubuntu:24.04
FROM ubuntu:24.04

#intall curl
RUN apt-get update && apt-get install -y curl

#copy the script into the image
COPY script.sh /usr/local/bin/script.sh

#make the script executable 
RUN chmod +x /usr/local/bin/script.sh

#set it to run on contianer start using CMD
CMD ["/usr/local/bin/script.sh"]


