FROM debian

RUN apt-get -y update && apt-get -y upgrade && \
	apt-get -y install wget bzip2 && \
	wget http://dl.4players.de/ts/releases/3.0.13.8/teamspeak3-server_linux_amd64-3.0.13.8.tar.bz2 && \
	tar xfv teamspeak3-server_linux_amd64-3.0.13.8.tar.bz2

EXPOSE	9987/UDP
EXPOSE	30033
EXPOSE	10011

CMD ["sh", "teamspeak3-server_linux_amd64/ts3server_minimal_runscript.sh"]




# docker build -t team_a .


# docker run -d --restart=always --name teamspeak \
#  -p 9987:9987/udp -p 30033:30033 -p 10011:10011 \
#  -v ${TS_VOLUME}:/teamspeak \
#  team_a

# d logs -f tem_a

# Teamspeak server: 192.168.99.100:9987
