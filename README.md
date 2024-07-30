# k8s-infra

## Project description
Kubernetes를 구축하는데 필요한 설정들을 정리해놓은 Repository입니다.

### metrics-hpa.yaml
k8s의 metric 서버에 대한 hpa를 명시하였습니다<br/>
ps. 실제로 동작할 일은 거의 없습니다.<br/>
[공식 docs](https://github.com/kubernetes-sigs/metrics-server) 기준 v0.5.0에서 100개의 Node 지표를 수집하는데 필요한 resource는 cpu: 100m, memory: 200MiB입니다.
|Quantity|Namespace threshold|Cluster threshold|
|------|---|---|
|#Nodes|n/a|100|
|#Pods per node|70|70|
|#Deployments with HPAs|100|100|
