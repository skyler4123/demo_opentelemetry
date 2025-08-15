# README

Docker Image https://hub.docker.com/r/grafana/otel-lgtm

### Run and access:
```
  docker run -p 3000:3000 -p 4317:4317 -p 4318:4318 --rm -ti grafana/otel-lgtm
```
```
  env OTEL_EXPORTER_OTLP_ENDPOINT="http://localhost:4318" rails server -p 8080
```
```
  http://127.0.0.1:8080/
```
```
  http://localhost:3000/a/grafana-lokiexplore-app/explore?patterns=%5B%5D&var-primary_label=service_name%7C%3D~%7C.%2B&from=now-15m&to=now&timezone=browser&var-lineFormat=&var-ds=loki&var-filters=&var-fields=&var-levels=&var-metadata=&var-jsonFields=&var-all-fields=&var-patterns=&var-lineFilterV2=&var-lineFilters=&var-filters_replica=
```