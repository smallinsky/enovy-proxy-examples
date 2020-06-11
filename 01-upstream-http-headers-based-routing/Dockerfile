FROM envoyproxy/envoy-alpine:v1.14.1
RUN apk add --no-cache ca-certificates
CMD /usr/local/bin/envoy -c /etc/envoy.yaml -l debug --service-cluster proxy
