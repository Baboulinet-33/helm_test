The error:

```shell
helm template test .
```
```txt
Error: template: test/charts/redis/templates/replicas/serviceaccount.yaml:13:14: executing "test/charts/redis/templates/replicas/serviceaccount.yaml" at <include "common.labels.standard" (dict "customLabels" .Values.commonLabels "context" $)>: error calling include: template: test/charts/etcd/charts/common/templates/_labels.tpl:6:27: executing "common.labels.standard" at <include "common.names.name" .>: error calling include: template: test/charts/etcd/charts/common/templates/_names.tpl:6:18: executing "common.names.name" at <.Chart.Name>: nil pointer evaluating interface {}.Name
```
