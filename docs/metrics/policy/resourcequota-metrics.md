# ResourceQuota Metrics

| Metric name                    | Metric type | Description                                                                                                               | Labels/tags                                                                                                                                         | Status       |
| ------------------------------ | ----------- | ------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| kube_resourcequota             | Gauge       |                                                                                                                           | `resourcequota`=&lt;quota-name&gt; <br> `namespace`=&lt;namespace&gt; <br> `resource`=&lt;ResourceName&gt; <br> `type`=&lt;quota-type&gt;           | STABLE       |
| kube_resourcequota_created     | Gauge       |                                                                                                                           | `resourcequota`=&lt;quota-name&gt; <br> `namespace`=&lt;namespace&gt;                                                                               | STABLE       |
| kube_resourcequota_annotations | Gauge       | Kubernetes annotations converted to Prometheus labels controlled via [--metric-annotations-allowlist](../../developer/cli-arguments.md) | `resourcequota`=&lt;quota-name&gt; <br> `namespace`=&lt;namespace&gt; <br> `annotation_RESOURCE_QUOTA_ANNOTATION`=&lt;RESOURCE_QUOTA_ANNOTATION&gt; | EXPERIMENTAL |
| kube_resourcequota_labels      | Gauge       | Kubernetes labels converted to Prometheus labels controlled via [--metric-labels-allowlist](../../developer/cli-arguments.md)           | `resourcequota`=&lt;quota-name&gt; <br> `namespace`=&lt;namespace&gt; <br> `label_RESOURCE_QUOTA_LABEL`=&lt;RESOURCE_QUOTA_LABEL&gt;                | EXPERIMENTAL |