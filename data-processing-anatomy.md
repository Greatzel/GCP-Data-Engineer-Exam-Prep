# Data Processing Anatomy

### Representation
Data Representation is how the data is formatted, stored, and managed.

Example:
- The data is stored in Google Big Query, and one way of managing it is imposing a 14 day lifespan on unused tables to save on cloud costs. One way data is formatted in a form of a file would be Parquet.

### Pipeline
Is the process that data goes through to move from one system to another.

Example:
- Every week our team sends data from Google Cloud Storage to our business partner's AWS S3 bucket. We do this by writing a DAG using a gcs_to_s3.

### Infrastructure
Is the overall foundation both software and hardware that the process to gather, move, and transform data is built on top upon.

Example:
- In Google, they have data centers filled with servers, and all these servers across multiple regions in the world, come together to be known as the "cloud". Clients purchase services from Google Cloud to run their data needs.



# Elements of GCP that make up the Data Processing Platform

### Storage and Databases
Where data is stored with will multiple storage and retrieval methods.

Example:
- Google Cloud Storage (GCS)

### Server-Based Processing
Makes use of the data that is stored to perform operations.

Example:
- Cloud Function that runs code that queries a Google Bigquery (GBq) table

### Integrated- Services (data + processing)
A combination of Storage and Databases, and Server-Based Processing for a streamlined data process.

Example:
- When the client logs in, the event will trigger a Cloud Function to run and retrieve the client's data from Google Bigquery. 
