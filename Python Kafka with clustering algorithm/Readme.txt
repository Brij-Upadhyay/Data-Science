Notes:
1.	Architecture: In the code random data will be generated after every 0.5 sec  which will generate random movement of the person and if the person will come near pizza centre
It will produce a message using Kafka producer
once the data will producer produce the data kafka consumer will get the data and using cluster.csv and customer.csv file it will generate the offer which was set looking in to clustering graphs
2.	Components:   Kafka Consumer/producer for real time messaging,
3.	Data flow
1. Raw data extracted from the csv file in dataframe
2. processed through EDA
3. Processed data sent to K mean clustering algorithm
4. clustering algorithm generate cluster_df.csv file which has data and cluster information
5. we will also generate random mobile no. data and save in csv file
6.kafka produce will randomly generate the data of the person location 
if person come near the shop it will send the message to consumer to extract the data and send offer message to customer mobile(simulation)
