#### 1- Create an Atlas Account
##### In this lab, you will create an Atlas account.

The atlas auth login command displays the one of the following messages in the console output when you have successfully authenticated.


```bash
atlas auth login
```
If you have a single project associated with your Atlas Account:

If you have multiple projects associated with your Atlas Account:

```shell
Successfully logged in as {Your Email Address}.
```

#### 2- Deploy an Atlas Cluster
##### In this lab, you will deploy an Atlas cluster to your Atlas account.

```shell
atlas setup --clusterName myAtlasClusterEDU --provider AWS --currentIp --skipSampleData --username myAtlasDBUser --password myatlas-001 --projectId 66a88de69f7ce476c83cde18    | tee atlas_cluster_details.txt
```

#### 3- Load the Sample Dataset Into Your Atlas Cluster
##### In this lab, you will load the sample dataset into your Atlas cluster.

```shell
atlas clusters sampleData load myAtlasClusterEDU
```

```shell
root@mongodb:/app# atlas clusters sampleData load myAtlasClusterEDU
Sample Data Job 63777f4360b9402aa143eb0f created.
```