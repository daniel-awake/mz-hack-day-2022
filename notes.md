 ```
 sudo semanage fcontext -a -t  container_file_t "/tmp/mz-hack-day-2022/sample_project/dbt(/.*)?"
restorecon -R .
```
for
```
root@ced90fbac93e:/usr/app/dbt# dbt debug
18:21:52  Encountered an error:
[Errno 13] Permission denied: '/root/.dbt/profiles.yml'
```
