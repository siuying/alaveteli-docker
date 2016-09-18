# alaveteli-docker

Dockerfile for building Alaveteli

You need:

1. Prepare config files database.yml, general.yml and newrelic.yml

Run with docker like this:

```
docker --run -v /data/alaveteli:/data/alaveteli \
  -v /opt/alaveteli/config/database.yml: /opt/alaveteli/config/database.yml \
  -v /opt/alaveteli/config/general.yml: /opt/alaveteli/config/general.yml \
  -v /opt/alaveteli/config/newrelic.yml: /opt/alaveteli/config/newrelic.yml \
  siuying/alaveteli
```

### How to customise:

`git clone https://github.com/siuying/alaveteli-docker.git`

`cd alaveteli-docker`

`docker build -t siuying/alaveteli .`
