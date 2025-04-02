# This is working Elastic search, Fluent Bit and Kibana stack deployed on Minikube in windows

1. Fluent bit is enabled to collect logs from kube-* along with some fitlering. Separate parsers.config is present
2. Elastic search collects the logs from fluent bit
3. Kibana is responsible for fetching the logs from elastic search
4. Stack management is reponsible for adding the index pattern of elastic search with logstash-* which is defined in fluent bit configuration file.
5. In discover section, you can see the logs.
