#Download base image from known working elasticsearch image
FROM elasticsearch:2.4.6
 
# Update Software repository
RUN apt-get update

#get libraries
RUN apt-get install wget


#set up the config since the base only uses the network binding, we need clustering and zen discovery
RUN wget <your elasticsearch yaml file for config>
RUN rm /usr/share/elasticsearch/config/elasticsearch.yml
RUN mv elasticsearch.yml /usr/share/elasticsearch/config/elasticsearch.yml
