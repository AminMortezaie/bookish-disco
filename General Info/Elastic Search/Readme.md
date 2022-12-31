# Elastic Search
Elasticsearch is a modern, distributed, and analytics search engine that is based or built on Apache Lucene. ElasticSearch enables you to store, search, and analyze vast or huge amounts of data in near real-time, providing results in milliseconds.
<br/>

As opposed to most NoSQL databases, Elasticsearch NoSQL focuses more on search capabilities and provides a rich HTTP RESTful API that allows for fast searches in near real-time.

## Advantages of ElasticSearch
- **Elasticsearch is a fast search engine** <br/>
Elasticsearch a good choice for time-sensitive use cases such as infrastructure monitoring and security analytics.

- **Elasticsearch is a distributed search engine<br/>**
Elasticsearch stores or distributes documents across several containers called shards, which are duplicated to provide redundant copies of the data in the event of a hardware or system failure. 
<br/>Due to Elasticsearch's distributed nature, it can scale up to thousands of servers and can handle petabytes of data.

- **Data ingestion, visualization, and reporting are simplified**<br/>
Data can be collected and processed easily using Beats and
Logstash before being indexed in Elasticsearch.Kibana provides UIs for quick access to log files, application performance monitoring (APM), and infrastructure metrics data.'

## ElasticSearch Usecases
Elasticsearch's speed and scalability as well as its ability to index different types of data make it ideal for a number of use cases. In addition to its high scalability, Elasticsearch also offers near-real-time search capabilities.<br/>

it is typically the underlying technology for applications requiring complex search
requirements.

## How does Elastic Search work?
- Gathering raw data from log files, system metrics or web apps.
- Normalizing and analyzing raw data.
- Send normalizied raw data to be indexed in Elastic search.
- Users can run queries.
- From Kibana,  users can create powerful visualizations of data, and visualize complex queries through interactive diagrams

## Different Data Types in Elastic Search
- Common data types
    - Binary
    - Boolean
    - Keywords: The keyword family, which includes the keyword, constant keyword ,and wildcard.
    - Numbers
    - Dates
    - Alias: Represents the alias of an existing field.

- Objects and relational types
    - Object: Represent a JSON object.
    - Nested: A JSON object that maintains a relationship between its subfields.
    - Flattened: An entire JSON object represented by a single field value.
    - Join: Establishes a parent/child relationship between documents within an index.

- Structured and Spatial data types
    - Range: Range types, like date_range, long_range float_range, double_range, and IP_range.
    - Point: Arbitrary cartesian points.
    - Geo_point: Longitude and latitude points
    - Shape: Arbitrary cartesian geometries.
    - Geo_shape: Complex shapes like polygons.

## Stoping Elastic Search on Ubuntu
You will need to 'kill' the running process. It is accomplished by sending a SIGTERM request to the process, which ends or terminates it. In order to initiate the shutdown process, you must first determine the process identifier (PID) for the Elasticsearch service you wish to terminate. Grep command can be used to locate processes easily.

## Elastic Search Mapping
ElasticSearch mappings define how documents and their fields are indexed and stored in ElasticSearch databases or ElasticSearch DBs.This defines the types and formats of the fields that appear in the documents. It refers to indexing.
<br/>

### Types of mapping
- **Static mapping:** Users perform static mappings when they create an index. We use static mappings to define data types and indexes.

- **Dynamic mapping:** Elasticsearch automatically creates dynamic mappings for the tables. The dynamic mapping of Elasticsearch comes in handy when we need to store extra attributes on documents. It is not always necessary to configure field names and types when indexing documents, as these will be created automatically by Elasticsearch based on any predefined rules.


## Elastic Search Fuzzy Search
With fuzzy search, you can find documents with terms similar to your search term based on a Levenshtein edit distance measure.
- Change one character (box → fox)
- Remove one character (black → lack)
- Insert one character (sic → sick)
- Transpose two adjacent characters (act → cat)

Within a specific edit distance, the fuzzy query generates a list of all possible variations and expansions of the search term. After that, the query returns a list of all possible matches. The most relevant and exact matches appear near the top of the list.

# Clusters in Elastic Search
A cluster is a collection of connected nodes. If you run only one instance or node of Elasticsearch, then you have a single-node cluster or a cluster of one node.<br/>

Clusters automatically reorganize themselves when nodes join or leave so the data is distributed evenly among all the nodes. Despite being fully functional, the cluster is at risk of data loss if it fails.

![](./elastic-cluster.png)