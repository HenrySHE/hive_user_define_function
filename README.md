# User Define Function in Hive (UDF)

[Reference Tutorial Link from Microsoft](https://docs.microsoft.com/en-us/azure/hdinsight/hadoop/apache-hadoop-hive-java-udf )

The process of using udf function:
1. New a maven project, and add dependencies:
    ```xml
    <dependencies>
        <dependency>
            <groupId>org.apache.hadoop</groupId>
            <artifactId>hadoop-client</artifactId>
            <version>2.7.3</version>
            <scope>provided</scope>
        </dependency>
        <dependency>
            <groupId>org.apache.hive</groupId>
            <artifactId>hive-exec</artifactId>
            <version>1.2.1</version>
            <scope>provided</scope>
        </dependency>
    </dependencies>
    ```

2. Create a class, and write your own function like "lowercase" function

3. Using maven to build a jar package

4. Copy the `.jar` file to `HDFS`

5. Load the jarfile as a function, then you can use the function in `HiveQL`



-----

**TODO:**
- Add more use cases [x]