## Some functional programming sample code snippets in java

```java
jobs.getJobNames().forEach(name -> log.info("job name: {}", name));
```

```java
jobs.getJobInstances(JOB_NAME, 0, jobs.getJobInstanceCount(JOB_NAME)).forEach(
 jobInstance -> {
                log.info("job instance id {}", jobInstance.getInstanceId());
            }
        );
 ```
