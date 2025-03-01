[comment]: # (AUTOGENERATED MARKDOWN CONTENT. UPDATES TO ODM DOCUMENTATION SHOULD BE DONE THROUGH ASSEMBLYLINE-BASE REPO!)
# ServiceDelta
> Service Delta relative to Initial Service Configuration

| Field | Type | Description | Required | Default |
| :--- | :--- | :--- | :--- | :--- |
| accepts | Keyword | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| rejects | Keyword | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| category | Keyword | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| classification | ClassificationString | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| config | Mapping [String, Any] | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| description | Text | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| default_result_classification | ClassificationString | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| enabled | Boolean | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| is_external | Boolean | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| licence_count | Integer | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| max_queue_length | Integer | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| min_instances | Integer | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| uses_tags | Boolean | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| uses_tag_scores | Boolean | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| uses_temp_submission_data | Boolean | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| uses_metadata | Boolean | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| name | Keyword | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| version | Keyword | Refer to:<br>[Service](../service/#service) | :material-checkbox-marked-outline: Yes | `None` |
| privileged | Boolean | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| disable_cache | Boolean | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| stage | Keyword | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| submission_params | List [[SubmissionParamsDelta](/assemblyline4_docs/odm/models/service_delta/#submissionparamsdelta)] | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| timeout | Integer | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| docker_config | [DockerConfigDelta](/assemblyline4_docs/odm/models/service_delta/#dockerconfigdelta) | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |
| dependencies | Mapping [String, [DependencyConfigDelta](/assemblyline4_docs/odm/models/service_delta/#dependencyconfigdelta)] | Refer to:<br>[Service](../service/#service) | :material-checkbox-marked-outline: Yes | See [DependencyConfigDelta](/assemblyline4_docs/odm/models/service_delta/#dependencyconfigdelta) for more details. |
| update_channel | Enum | Refer to:<br>[Service](../service/#service)<br>Values:<br>`"beta", "dev", "rc", "stable"` | :material-minus-box-outline: Optional | `None` |
| update_config | [UpdateConfigDelta](/assemblyline4_docs/odm/models/service_delta/#updateconfigdelta) | Refer to:<br>[Service](../service/#service) | :material-minus-box-outline: Optional | `None` |


[comment]: # (AUTOGENERATED MARKDOWN CONTENT. UPDATES TO ODM DOCUMENTATION SHOULD BE DONE THROUGH ASSEMBLYLINE-BASE REPO!)
## DependencyConfigDelta
> None

| Field | Type | Description | Required | Default |
| :--- | :--- | :--- | :--- | :--- |
| container | [DockerConfigDelta](/assemblyline4_docs/odm/models/service_delta/#dockerconfigdelta) | Refer to:<br>[Service - DependencyConfig](../service/#dependencyconfig) | :material-minus-box-outline: Optional | `None` |
| volumes | Mapping [String, [PersistentVolumeDelta](/assemblyline4_docs/odm/models/service_delta/#persistentvolumedelta)] | Refer to:<br>[Service - DependencyConfig](../service/#dependencyconfig) | :material-checkbox-marked-outline: Yes | See [PersistentVolumeDelta](/assemblyline4_docs/odm/models/service_delta/#persistentvolumedelta) for more details. |
| run_as_core | Boolean | Refer to:<br>[Service - DependencyConfig](../service/#dependencyconfig) | :material-minus-box-outline: Optional | `None` |


[comment]: # (AUTOGENERATED MARKDOWN CONTENT. UPDATES TO ODM DOCUMENTATION SHOULD BE DONE THROUGH ASSEMBLYLINE-BASE REPO!)
### DockerConfigDelta
> Docker Configuration Delta

| Field | Type | Description | Required | Default |
| :--- | :--- | :--- | :--- | :--- |
| allow_internet_access | Boolean | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig) | :material-minus-box-outline: Optional | `None` |
| command | List [Keyword] | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig) | :material-minus-box-outline: Optional | `None` |
| cpu_cores | Float | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig) | :material-minus-box-outline: Optional | `None` |
| environment | List [[EnvironmentVariable](/assemblyline4_docs/odm/models/service_delta/#environmentvariable)] | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig) | :material-minus-box-outline: Optional | `None` |
| image | Keyword | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig) | :material-minus-box-outline: Optional | `None` |
| registry_username | Keyword | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig) | :material-minus-box-outline: Optional | `` |
| registry_password | Keyword | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig) | :material-minus-box-outline: Optional | `` |
| registry_type | Enum | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig)<br>Values:<br>`"docker", "harbor"` | :material-minus-box-outline: Optional | `None` |
| ports | List [Keyword] | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig) | :material-minus-box-outline: Optional | `None` |
| ram_mb | Integer | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig) | :material-minus-box-outline: Optional | `None` |
| ram_mb_min | Integer | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig) | :material-minus-box-outline: Optional | `None` |
| service_account | Keyword | None | :material-minus-box-outline: Optional | `None` |


[comment]: # (AUTOGENERATED MARKDOWN CONTENT. UPDATES TO ODM DOCUMENTATION SHOULD BE DONE THROUGH ASSEMBLYLINE-BASE REPO!)
#### EnvironmentVariable
> None

| Field | Type | Description | Required | Default |
| :--- | :--- | :--- | :--- | :--- |
| name | Keyword | Refer to:<br>[Service - Enviroment Variable](../service/#environmentvariable) | :material-checkbox-marked-outline: Yes | `None` |
| value | Keyword | Refer to:<br>[Service - Enviroment Variable](../service/#environmentvariable) | :material-checkbox-marked-outline: Yes | `None` |


[comment]: # (AUTOGENERATED MARKDOWN CONTENT. UPDATES TO ODM DOCUMENTATION SHOULD BE DONE THROUGH ASSEMBLYLINE-BASE REPO!)
### PersistentVolumeDelta
> None

| Field | Type | Description | Required | Default |
| :--- | :--- | :--- | :--- | :--- |
| mount_path | Keyword | Refer to:<br>[Service - PeristentVolume](../service/#persistentvolume) | :material-minus-box-outline: Optional | `None` |
| capacity | Keyword | Refer to:<br>[Service - PeristentVolume](../service/#persistentvolume) | :material-minus-box-outline: Optional | `None` |
| storage_class | Keyword | Refer to:<br>[Service - PeristentVolume](../service/#persistentvolume) | :material-minus-box-outline: Optional | `None` |
| access_mode | Enum | Refer to:<br>[Service - PeristentVolume](../service/#persistentvolume)<br>Values:<br>`"ReadWriteMany", "ReadWriteOnce"` | :material-minus-box-outline: Optional | `None` |


[comment]: # (AUTOGENERATED MARKDOWN CONTENT. UPDATES TO ODM DOCUMENTATION SHOULD BE DONE THROUGH ASSEMBLYLINE-BASE REPO!)
## DockerConfigDelta
> Docker Configuration Delta

| Field | Type | Description | Required | Default |
| :--- | :--- | :--- | :--- | :--- |
| allow_internet_access | Boolean | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig) | :material-minus-box-outline: Optional | `None` |
| command | List [Keyword] | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig) | :material-minus-box-outline: Optional | `None` |
| cpu_cores | Float | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig) | :material-minus-box-outline: Optional | `None` |
| environment | List [[EnvironmentVariable](/assemblyline4_docs/odm/models/service_delta/#environmentvariable)] | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig) | :material-minus-box-outline: Optional | `None` |
| image | Keyword | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig) | :material-minus-box-outline: Optional | `None` |
| registry_username | Keyword | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig) | :material-minus-box-outline: Optional | `` |
| registry_password | Keyword | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig) | :material-minus-box-outline: Optional | `` |
| registry_type | Enum | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig)<br>Values:<br>`"docker", "harbor"` | :material-minus-box-outline: Optional | `None` |
| ports | List [Keyword] | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig) | :material-minus-box-outline: Optional | `None` |
| ram_mb | Integer | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig) | :material-minus-box-outline: Optional | `None` |
| ram_mb_min | Integer | Refer to:<br>[Service - DockerConfig](../service/#dockerconfig) | :material-minus-box-outline: Optional | `None` |
| service_account | Keyword | None | :material-minus-box-outline: Optional | `None` |


[comment]: # (AUTOGENERATED MARKDOWN CONTENT. UPDATES TO ODM DOCUMENTATION SHOULD BE DONE THROUGH ASSEMBLYLINE-BASE REPO!)
### EnvironmentVariable
> None

| Field | Type | Description | Required | Default |
| :--- | :--- | :--- | :--- | :--- |
| name | Keyword | Refer to:<br>[Service - Enviroment Variable](../service/#environmentvariable) | :material-checkbox-marked-outline: Yes | `None` |
| value | Keyword | Refer to:<br>[Service - Enviroment Variable](../service/#environmentvariable) | :material-checkbox-marked-outline: Yes | `None` |


[comment]: # (AUTOGENERATED MARKDOWN CONTENT. UPDATES TO ODM DOCUMENTATION SHOULD BE DONE THROUGH ASSEMBLYLINE-BASE REPO!)
## SubmissionParamsDelta
> None

| Field | Type | Description | Required | Default |
| :--- | :--- | :--- | :--- | :--- |
| default | Any | Refer to:<br>[Service - SubmissionParams](../service/#submissionparams) | :material-minus-box-outline: Optional | `None` |
| name | Keyword | Refer to:<br>[Service - SubmissionParams](../service/#submissionparams) | :material-minus-box-outline: Optional | `None` |
| type | Enum | Refer to:<br>[Service - SubmissionParams](../service/#submissionparams)<br>Values:<br>`"bool", "int", "list", "str"` | :material-minus-box-outline: Optional | `None` |
| value | Any | Refer to:<br>[Service - SubmissionParams](../service/#submissionparams) | :material-minus-box-outline: Optional | `None` |
| list | Any | Refer to:<br>[Service - SubmissionParams](../service/#submissionparams) | :material-minus-box-outline: Optional | `None` |
| hide | Boolean | Refer to:<br>[Service - SubmissionParams](../service/#submissionparams) | :material-minus-box-outline: Optional | `None` |


[comment]: # (AUTOGENERATED MARKDOWN CONTENT. UPDATES TO ODM DOCUMENTATION SHOULD BE DONE THROUGH ASSEMBLYLINE-BASE REPO!)
## UpdateConfigDelta
> None

| Field | Type | Description | Required | Default |
| :--- | :--- | :--- | :--- | :--- |
| generates_signatures | Boolean | Refer to:<br>[Service - UpdateConfig](../service/#updateconfig) | :material-minus-box-outline: Optional | `None` |
| sources | List [[UpdateSourceDelta](/assemblyline4_docs/odm/models/service_delta/#updatesourcedelta)] | Refer to:<br>[Service - UpdateConfig](../service/#updateconfig) | :material-minus-box-outline: Optional | `None` |
| update_interval_seconds | Integer | Refer to:<br>[Service - UpdateConfig](../service/#updateconfig) | :material-minus-box-outline: Optional | `None` |
| wait_for_update | Boolean | Refer to:<br>[Service - UpdateConfig](../service/#updateconfig) | :material-minus-box-outline: Optional | `None` |
| signature_delimiter | Enum | Refer to:<br>[Service - UpdateConfig](../service/#updateconfig)<br>Values:<br>`"comma", "custom", "double_new_line", "file", "new_line", "none", "pipe", "space"` | :material-minus-box-outline: Optional | `None` |
| custom_delimiter | Keyword | Refer to:<br>[Service - UpdateConfig](../service/#updateconfig) | :material-minus-box-outline: Optional | `None` |


[comment]: # (AUTOGENERATED MARKDOWN CONTENT. UPDATES TO ODM DOCUMENTATION SHOULD BE DONE THROUGH ASSEMBLYLINE-BASE REPO!)
### UpdateSourceDelta
> None

| Field | Type | Description | Required | Default |
| :--- | :--- | :--- | :--- | :--- |
| name | Keyword | Refer to:<br>[Service - UpdateSource](../service/#updatesource) | :material-minus-box-outline: Optional | `None` |
| password | Keyword | Refer to:<br>[Service - UpdateSource](../service/#updatesource) | :material-minus-box-outline: Optional | `` |
| pattern | Keyword | Refer to:<br>[Service - UpdateSource](../service/#updatesource) | :material-minus-box-outline: Optional | `` |
| private_key | Keyword | Refer to:<br>[Service - UpdateSource](../service/#updatesource) | :material-checkbox-marked-outline: Yes | `` |
| ca_cert | Keyword | Refer to:<br>[Service - UpdateSource](../service/#updatesource) | :material-minus-box-outline: Optional | `` |
| ssl_ignore_errors | Boolean | Refer to:<br>[Service - UpdateSource](../service/#updatesource) | :material-checkbox-marked-outline: Yes | `False` |
| proxy | Keyword | Refer to:<br>[Service - UpdateSource](../service/#updatesource) | :material-minus-box-outline: Optional | `` |
| uri | Keyword | Refer to:<br>[Service - UpdateSource](../service/#updatesource) | :material-minus-box-outline: Optional | `None` |
| username | Keyword | Refer to:<br>[Service - UpdateSource](../service/#updatesource) | :material-minus-box-outline: Optional | `` |
| headers | List [[EnvironmentVariable](/assemblyline4_docs/odm/models/service_delta/#environmentvariable)] | Refer to:<br>[Service - UpdateSource](../service/#updatesource) | :material-minus-box-outline: Optional | `None` |
| default_classification | Classification | Refer to:<br>[Service - UpdateSource](../service/#updatesource) | :material-minus-box-outline: Optional | `None` |
| git_branch | Keyword | Refer to:<br>[Service - UpdateSource](../service/#updatesource) | :material-minus-box-outline: Optional | `` |
| sync | Boolean | Refer to:<br>[Service - UpdateSource](../service/#updatesource) | :material-minus-box-outline: Optional | `False` |


[comment]: # (AUTOGENERATED MARKDOWN CONTENT. UPDATES TO ODM DOCUMENTATION SHOULD BE DONE THROUGH ASSEMBLYLINE-BASE REPO!)
#### EnvironmentVariable
> None

| Field | Type | Description | Required | Default |
| :--- | :--- | :--- | :--- | :--- |
| name | Keyword | Refer to:<br>[Service - Enviroment Variable](../service/#environmentvariable) | :material-checkbox-marked-outline: Yes | `None` |
| value | Keyword | Refer to:<br>[Service - Enviroment Variable](../service/#environmentvariable) | :material-checkbox-marked-outline: Yes | `None` |


