# AWS_Fargate_Promethe_Graphana_Install
AWS_Fargate_Promethe_Graphana_Install


# Followed AWS doc for installation Prometheus and Grafana

https://aws.amazon.com/blogs/containers/monitoring-amazon-eks-on-aws-fargate-using-prometheus-and-grafana/

helm install prometheus -f prometheus_values.yml   prometheus-community/prometheus --version 21.0.1 --namespace prometheus
helm install grafana -f grafana-values.yaml \
  grafana/grafana --namespace prometheus

# Prometheus url e erişmek için ;

1) Aşağıdaki Prometheus port yönlendirme komutunu koş 

kubectl --namespace prometheus port-forward prometheus-server-7488978d49-vsdrg 9090

2) Sonra şu linke git : http://localhost:9090
