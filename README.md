# Frequent Itemset Analysis on Amazon Metadata

# Group Members
Ali Tanveer (21I-1692)
Afza Anjum (21I-1724)
Ruwaid Imran (21I-1728)

##Introduction
Frequent Itemset Analysis is a data mining technique used to discover interesting patterns in large datasets. 
In the context of Amazon Metadata, it can be applied to identify frequent combinations of items purchased together, which can be valuable for market basket analysis and personalized recommendations.

## 1. Pre-Processing
Loaded the Sampled Amazon dataset.
Preprocessed the data to clean and format it for analysis, ensuring suitability for streaming and frequent itemset mining.
Generated a new JSON file containing the preprocessed data.
Implemented batch processing to execute pre-processing in real-time.

## 2. Streaming Pipeline Setup
Developed a producer application that streams the preprocessed data in real-time.
Created three consumer applications that subscribe to the producer's data stream.

## 3. Frequent Itemset Mining
Implemented the Apriori algorithm in one consumer, providing real-time insights and associations.
Implemented the PCY algorithm in one consumer, displaying real-time insights and associations.
Developed an innovative approach in the third consumer, showcasing creativity and uniqueness. This consumer was designed to hold the highest number of marks.

## 4. Challenges and Solutions
Adapting Apriori and PCY algorithms to a streaming context posed challenges due to the need for access to the entire dataset. 
To address this, we employed a sliding window approach, allowing us to process data in chunks and adapt the algorithms for real-time analysis.

## 5. Database Integration
Chose MongoDB as the database for storing results.
Modified each consumer to connect to MongoDB and store the results, ensuring data persistence and scalability.

## Conclusion
This project demonstrates the effective use of Apache Kafka and Python for real-time data analysis. 
By implementing innovative approaches to adapt traditional algorithms to a streaming environment, we were able to perform frequent itemset mining and gain valuable insights from streaming data.
The integration with MongoDB provides a scalable solution for storing and analyzing large volumes of data in real-time.
