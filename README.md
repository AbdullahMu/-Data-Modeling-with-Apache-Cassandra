
<h1 id="project-data-modeling-with-cassandra">Project: Data Modeling with Cassandra</h1>
<p>A startup called Sparkify wants to analyze the data they’ve been collecting on songs and user activity on their new music streaming app. The analysis team is particularly interested in understanding what songs users are listening to. Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app.</p>
<p>They’d like a data engineer to create an Apache Cassandra database which can create queries on song play data to answer the questions, and wish to bring you on the project. Your role is to create a database for this analysis. You’ll be able to test your database by running queries given to you by the analytics team from Sparkify to create the results.</p>
<h2 id="project-overview">Project Overview</h2>
<p>In this project, you’ll apply what you’ve learned on data modeling with Apache Cassandra and complete an ETL pipeline using Python. To complete the project, you will need to model your data by creating tables in Apache Cassandra to run queries. You are provided with part of the ETL pipeline that transfers data from a set of CSV files within a directory to create a streamlined CSV file to model and insert data into Apache Cassandra tables.</p>
<p>We have provided you with a project template that takes care of all the imports and provides a structure for ETL pipeline you’d need to process this data.</p>
<h2 id="datasets">Datasets</h2>
<p>For this project, you’ll be working with one dataset:  <code>event_data</code>. The directory of CSV files partitioned by date. Here are examples of filepaths to two files in the dataset:</p>
<pre><code>event_data/2018-11-08-events.csv
event_data/2018-11-09-events.csv
</code></pre>
<h2 id="project-template">Project Template</h2>
<p>To get started with the project, go to the workspace on the next page, where you’ll find the project template (a Jupyter notebook file). You can work on your project and submit your work through this workspace.</p>
<p>The project template includes one Jupyter Notebook file, in which:</p>
<ul>
<li>you will process the  <code>event_datafile_new.csv</code>  dataset to create a denormalized dataset</li>
<li>you will model the data tables keeping in mind the queries you need to run</li>
<li>you have been provided queries that you will need to model your data tables for</li>
<li>you will load the data into tables you create in Apache Cassandra and run your queries</li>
</ul>
<h1 id="project-steps">Project Steps</h1>
<p>Below are steps you can follow to complete each component of this project.</p>
<h3 id="modeling-your-nosql-database-or-apache-cassandra-database">Modeling your NoSQL database or Apache Cassandra database</h3>
<ol>
<li>Design tables to answer the queries outlined in the project template</li>
<li>Write Apache Cassandra  <code>CREATE KEYSPACE</code>  and  <code>SET KEYSPACE</code>  statements</li>
<li>Develop your  <code>CREATE</code>  statement for each of the tables to address each question</li>
<li>Load the data with  <code>INSERT</code>  statement for each of the tables</li>
<li>Include  <code>IF NOT EXISTS</code>  clauses in your  <code>CREATE</code>  statements to create tables only if the tables do not already exist. We recommend you also include  <code>DROP TABLE</code>  statement for each table, this way you can run drop and create tables whenever you want to reset your database and test your ETL pipeline</li>
<li>Test by running the proper select statements with the correct  <code>WHERE</code>  clause</li>
</ol>
<h3 id="build-etl-pipeline">Build ETL Pipeline</h3>
<ol>
<li>Implement the logic in section Part I of the notebook template to iterate through each event file in  <code>event_data</code>  to process and create a new CSV file in Python</li>
<li>Make necessary edits to Part II of the notebook template to include Apache Cassandra  <code>CREATE</code>  and  <code>INSERT</code>  statements to load processed records into relevant tables in your data model</li>
<li>Test by running  <code>SELECT</code>  statements after running the queries on your database</li>
</ol>
<blockquote>
<p>Written with <a href="https://stackedit.io/">StackEdit</a>.</p>
</blockquote>

