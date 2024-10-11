**ISchool Data Analytics on Course Registration and Curricular Data**

**Project Overview**:

This project focuses on creating various data analytics from course registration and curricular data. The aim is to work with distributed databases and systems, applying the knowledge learned throughout the course to solve real-world data science problems. The project utilizes technologies such as MongoDB, Minio, Cassandra, Elasticsearch, Kibana, Neo4j, and PySpark.

**Technologies Used**:

1.*PySpark*: For distributed data processing and transformations.

2.*MongoDB*: NoSQL database for storing course and student data.

3.*Minio*: S3-compatible object storage for enrollment data.

4.*Cassandra*: Distributed NoSQL database for storing wide data related to course sections.

5.*Elasticsearch*: Search engine for indexing course and enrollment data.

6.*Kibana*: Data visualization tool for creating dashboards and insights from Elasticsearch indices.

7.*Neo4j*: Graph database used for storing relationships between courses, programs, and prerequisites.

8.*Jupyter Lab*: Interactive environment for developing and running PySpark code.

*Key Accomplishments*:

*1. Data Integration and Preparation*:

Connected to MongoDB, Minio, Cassandra, Elasticsearch, and Neo4j using PySpark for reading and transforming both process-oriented and reference-oriented data.
Processed course registration and curricular data, including student enrollments and course sections, from the provided datasets.

*2. Data Preparation for Cassandra and Elasticsearch*:

Prepared the section data to be loaded into Cassandra and Elasticsearch by merging reference data from multiple sources, such as terms, courses, and program information.
Flattened nested data structures to facilitate loading into Elasticsearch, ensuring that all key attributes, such as course requirements and electives, were properly handled.

*3. Cassandra Table Design and Loading:*

Designed and created a Cassandra table named sections with an appropriate key structure to store course section data. The table schema ensured efficient querying for wide datasets.
Loaded the transformed data into Cassandra and demonstrated the correctness by querying back the data using PySpark.

*4. Elasticsearch Indexing and Queries:*

Loaded the prepared data into Elasticsearch under the sections and enrollments indices.
Queried Elasticsearch using PySpark to demonstrate the data was properly indexed and accessible, supporting real-time analytics and search capabilities.

*5. Neo4j Graph Construction:*

Created nodes in Neo4j for courses and programs, excluding unnecessary attributes like prerequisites and electives.
Established relationships between nodes, such as required and elective courses, and loaded them into Neo4j.
Demonstrated the relationships by querying the graph with Cypher queries.

*6. Data Visualization in Kibana:*

Built a student dashboard using Kibana from the enrollments index pattern, which provided detailed insights into individual students' GPA, courses taken, and credit completion.
Created a course dashboard to visualize course-related metrics, such as enrollment-to-capacity ratios, summaries of courses for a specific academic year, and counts of required vs. elective courses.
