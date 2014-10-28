---
layout: post
title:  "Sql Injection, NoSql vs Sql"
date:   2014-06-06 16:24:54
categories: jekyll update
---
![alt text][sql]

#### What is Sql Injection?

SQL injection is a common application layer web attack scheme used by hackers to steal data from companies. If you code is not done properly hackers are able to exploit your security vulnerability in an applications software by injecting SQL statements into an input field element on the website such as request forms, feedback forms, search bar, carts ect… These statements are sent to the backend database, if the proper code is not written to check these input SQL statements the attack will hackers to view information from the database or even wipe out all the data. As a new web developer the best way to prevent this would be to stop writing dynamic queries and/or prevent user supplied input which contains malicious SQL from affecting the logic of the executed query.

#### Sql vs NoSql

| Sql      | NoSql    
|----------|:----------------:|
|SQL databases are primarily called as Relational Databases (RDBMS)|NoSQL database are primarily called as non-relational or distributed database|
|SQL databases are table based databases whereas NoSQL databases are document based, key-value pairs, graph databases or wide-column stores.|NoSQL databases are the collection of key-value pair, documents, graph databases or wide-column stores which do not have standard schema definitions which it needs to adhered to.
|SQL databases have predefined schema|NoSQL databases have dynamic schema for unstructured data.
|SQL databases are vertically scalable|NoSQL databases are horizontally scalable.
|SQL databases uses SQL ( structured query language ) for defining and manipulating the data,|NoSQL database, queries are focused on collection of documents. Sometimes it is also called as UnQL (Unstructured Query Language).
|SQL databases are good fit for the complex query intensive environment|NoSQL databases are not good fit for complex queries. On a high-level, NoSQL don’t have standard interfaces to perform complex queries, and the queries themselves in NoSQL are not as powerful as SQL query language.
|SQL database examples: MySql, Oracle, Sqlite, Postgres and MS-SQL.|NoSQL database examples: MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb



#### Better Sql Queries

To retrieve data from the database we use SQL statements. When considering performance, the best query techniques should be used. There are a few ways to do this. 1. Indexing your column is a common way to optimize your search results. 2. Use the Symbol Operator such as >,<,=,!=, etc.

{% highlight ruby %}
SELECT * FROM TABLE WHERE COLUMN >= 15
{% endhighlight %}

Use of a postfix wildcard instead of pre or full wildcard '%'

{% highlight ruby %}
SELECT * FROM TABLE WHERE COLUMN LIKE 'hello%'
{% endhighlight %}

Use the LIKE, IN, EXIST or = symbol operator instead of a negative operator such as NOT LIKE, NOT IN, NOT EXIST or != symbol. Using a negative operator will cause the search to find every single row to identify that they are all not belong or exist with the table.

Use the count operator to determine whether a particular data exists.

{% highlight ruby %}
SELECT COLUMN FROM TABLE WHERE COUNT(COLUMN) > 0
{% endhighlight %}

Use index Unique column, Max and Min Operators, Select the most effecient data types possible and another would be to limit the result of the query.

{% highlight ruby %}
SELECT * FROM TABLE WHERE 1 LIMIT 10
{% endhighlight %}

[sql]: http://1.bp.blogspot.com/-QhOwiLtbSCg/UXwh3jz3SxI/AAAAAAAAARM/Ll9oHyb4Dxw/s1600/SQL+Injection.jpg "sql-image"