# Anomaly_Detection
Identifying anomalous agents behavior using clustering algorithms (Unsupervised Learning)

The objective of this project is to identify anomalous user behavior using unsupervised learning techniques from the given one month transaction history. Anomalous behavior can be based on the number of transactions handled by a particular user on a daily basis and the different types of events handled within each transaction.                                                                                                                                          

Introduction to Data:                                                                                   
The dataset comprises of transactional data pertaining to customer service calls from Sykes for one of their clients - Frontier Communications. It includes event data for the last 30 days from the date on which data is extracted. For the current analysis, we are using data which includes around 4.35 million records. Each customer call is a unique transaction. Each record in the data represents an occurrence of an event within a transaction. An event can be anything such as Answer call, Customer Put on hold, End call and so on. There are five variables in the dataset. 

They are as follows:                                                                                     
Transaction ID    Unique identifier for transactions                                                     
User Global ID    Unique identifier of each user. Here, user is a representative from Sykes working for Frontier Communications              Event Name        Description for the type of event                                                      
CreatedDateTime   Date and time at which the transaction occurred                                        
LOB ID            Line of Business Identifier                                                            
                                                                                                 
Approach:                                                                                                
To find out anomalous user behavior, I have first aggregated the data set on the date portion of the column 'Date' to calculate the total number of transactions and various events occurred per user ID on each day. I have done so, because performing a day-wise aggregation will enable us in finding out how frequently a specific user is exhibiting anomalous behavior. On this aggregated data, I have applied unsupervised learning techniques such as k-means, hierarchical and density-based clustering. Based on the clusters formed, I have identified outliers which are nothing but anomalous users Ids.
