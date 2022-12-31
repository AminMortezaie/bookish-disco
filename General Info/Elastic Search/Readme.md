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