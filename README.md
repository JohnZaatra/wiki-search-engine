# Wikipedia Search Engine

This project is a search engine built for English Wikipedia, designed to process queries and retrieve relevant articles from the entire corpus. The project was developed as part of a university course and is hosted on Google Cloud Platform (GCP), using Google Storage buckets for data storage and cloud computing resources for efficient indexing and retrieval.

## Project Overview

The Wikipedia Search Engine is capable of processing user queries and returning ranked results from a massive dataset—an entire English Wikipedia dump. The system was designed to be efficient and scalable, supporting various ranking methods for relevance, including cosine similarity, binary ranking by title and anchor text, PageRank, and article page views.

## Key Features

- **Efficient Retrieval:** Optimized for fast query processing with average retrieval times below 2 seconds.
- **Multiple Ranking Methods:** Implements five ranking methods, including:
  - Cosine similarity using tf-idf on the body of articles
  - Binary ranking using the title of articles
  - Binary ranking using anchor text
  - Ranking by PageRank
  - Ranking by article page views
- **Hosted on Google Cloud Platform (GCP):** The search engine is deployed using Compute Engine instances and Google Storage buckets for scalable data handling.
- **Fully Functional:** The search engine is accessible via a URL, allowing users to query the system and receive relevant results from the entire Wikipedia corpus.
- **Tested and Evaluated:** Extensive testing has been performed, including qualitative and quantitative evaluations of the engine's performance and ranking quality.

## Architecture

The search engine is built using Python with Flask for the frontend. It interacts with an inverted index built from the Wikipedia dump, which is stored in Google Storage buckets. The system processes queries using the defined ranking methods and retrieves results in real-time, making use of cloud-based computation resources to ensure high efficiency.

- **Frontend:** The search engine interface is built with Flask and hosted on a Compute Engine instance.
- **Backend:** Query processing and ranking algorithms are implemented in Python, utilizing cloud resources to handle the large Wikipedia dataset.
- **Storage:** Data is stored in Google Storage buckets, ensuring easy access to the Wikipedia dump and indexing data.

## Google Cloud Platform Setup

The project makes use of several GCP services:
- **Compute Engine:** The search engine runs on a GCP instance, providing the necessary computing power for query processing and ranking.
- **Google Storage Buckets:** The Wikipedia dump and index data are stored in GCP buckets, enabling efficient access and management of the dataset.
- **Cloud Deployment:** The project includes a script (`run_frontend_in_gcp.sh`) for deploying the search engine on GCP and running it on a public IP.

## Performance and Testing

- The project met the minimum performance requirements, processing queries in under 35 seconds. It also achieved a MAP@40 score greater than 0.25, meeting the quality criteria set by the course.
- During the two-day testing period, the search engine was fully operational, allowing users to test its functionality through the provided URL. The engine handled a variety of queries with accurate and relevant results.

## Conclusion

This project demonstrates the power of cloud computing for building and deploying large-scale search engines. By utilizing Google Cloud Platform, the system efficiently processes queries against a vast dataset (the entire English Wikipedia) while providing accurate and relevant search results.

The project can be accessed and used just like any other search engine, where users can submit queries and receive results in real time, just as one would with Google.

## Why This Project Stands Out

This Wikipedia Search Engine project is a significant achievement that demonstrates my ability to design and deploy a highly scalable, efficient system on Google Cloud Platform. By utilizing advanced search algorithms like tf-idf, PageRank, and custom ranking methods, I created an engine that processes large datasets with lightning-fast query responses, achieving impressive performance metrics. The project showcases my expertise in cloud infrastructure, data processing, and full-stack development, while also reflecting my ability to solve complex challenges in real-time search systems. This is a testament to my technical skills and my capacity to deliver high-quality, real-world solutions.

