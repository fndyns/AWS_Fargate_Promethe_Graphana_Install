# AWS_Fargate_Promethe_Graphana_Install
AWS_Fargate_Promethe_Graphana_Install

Prometheus port yönlendirme yap sonra şu linke git : http://localhost:9090

kubectl --namespace prometheus port-forward prometheus-server-7488978d49-vsdrg 9090


helm install prometheus -f prometheus_values.yml   prometheus-community/prometheus --version 21.0.1 --namespace prometheus


Followed AWS doc for installation Prometheus and Grafana

https://aws.amazon.com/blogs/containers/monitoring-amazon-eks-on-aws-fargate-using-prometheus-and-grafana/
