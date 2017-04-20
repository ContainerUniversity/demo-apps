# Parallel job with Work Queue

1) Create Redis Pod and Service
 
Then Exec into Redis POD so we can add some entries:

``` kubectl run -i --tty temp --image redis --command "/bin/sh" ```

For adding entries in queue:

```
> rpush job2 "banana"
> rpush job2 "apple" 
```

2) Now run the job from job.yml and execution of job will kick off
