# Udacity-Data-lakes-and-Lakehouses-with-Spark-and-Azure-Databricks
Course Data lakes and Lakehouses with Spark and Azure Databricks

# Azure Credentials

User: odl_user_303377@udacityhol.onmicrosoft.com

Access Pass:

*C^dYRBT


## Maps

In Spark, maps take data as input and then transform that data with whatever function you put in the map. They are like directions for the data telling how each input should get to the output.

The first code cell creates a SparkContext object. With the SparkContext, you can input a dataset and parallelize the data across a cluster (since you are currently using Spark in local mode on a single machine, technically the dataset isn't distributed yet).

### 
# You might have noticed this code in the screencast.
###
# import findspark
# findspark.init('spark-2.3.2-bin-hadoop2.7')
#
# The findspark Python module makes it easier to install
# Spark in local mode on your computer. This is convenient
# for practicing Spark syntax locally. 
# However, the workspaces already have Spark installed and you do not
# need to use the findspark module
#


"RDD" in the output refers to resilient distributed dataset. RDDs are exactly what they say they are: fault-tolerant datasets distributed across a cluster. This is how Spark stores data.

To get Spark to actually run the map step, you need to use an "action". One available action is the collect method. The collect() method takes the results from all of the clusters and "collects" them into a single list on the master node.


## Imperative VS Declarative Programming

We will cover two different ways to manipulate our data:

Imperative programming using Python and RDDs

Imperative programming is concerned with the How

Let's get in the car, drive two miles down the road to my favorite bakery, go into the shop, select the cake from the counter, purchase the cake, and then drive home.

Focus on the exact steps, how we get to the result

Data transformations with RDDs

## Declarative programming using DataFrames and SQL

Cares about the What
Let's get the cake for Julia.
Concerned about the result we want to achieve
Abstraction layer of an imperative system
If you have used pandas DataFrames before, you are probably familiar with how to manipulate DataFrames programmatically. We can chain methods such as filter and group by one after another, transforming the DataFrame further and further. In the next few videos, we will dive into how to do data transformations with DataFrames and declarative programming.
