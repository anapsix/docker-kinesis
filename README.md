# docker-kinesis
Spinup local Kinesis with Docker.
Actual local Kinesis server is by @mhart: https://github.com/mhart/kinesalite

## Usage
```
docker run -it --rm -p 4567:4567 -v /tmp/kinesis_db:/tmp/kinesis_db -e DB_PATH=/tmp/kinesis_db anapsix/kinesis
```

Options:
`USE_SSL`: enables `--ssl`
`DB_PATH`: enables `--path $DB_PATH`
`SHARD_LIMIT`: enables `--shardLimit $SHARD_LIMIT`