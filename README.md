# terraform-aws-elastic-beanstalk-application

Terraform module to provision AWS Elastic Beanstalk application




## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| appversion_lifecycle_delete_source_from_s3 | Whether to delete application versions from S3 source | bool | `false` | no |
| appversion_lifecycle_max_count | The max number of application versions to keep | number | `1000` | no |
| appversion_lifecycle_service_role_arn | The service role ARN to use for application version cleanup. If left empty, the `appversion_lifecycle` block will not be created | string | `` | no |
| attributes | Additional attributes (e.g. `1`) | list(string) | `<list>` | no |
| delimiter | Delimiter to be used between `name`, `namespace`, `stage`, etc. | string | `-` | no |
| description | Elastic Beanstalk Application description | string | `` | no |
| name | Solution name, e.g. 'app' or 'cluster' | string | - | yes |
| namespace | Namespace, which could be your organization name, e.g. 'eg' or 'cp' | string | `` | no |
| stage | Stage, e.g. 'prod', 'staging', 'dev', or 'test' | string | `` | no |
| tags | Additional tags (e.g. `map('BusinessUnit`,`XYZ`) | map(string) | `<map>` | no |



## Outputs

| Name | Description |
|------|-------------|
| elastic_beanstalk_application_name | Elastic Beanstalk Application name |




## Copyright
Copyright © 2020 [Ceibo IT](https://ceibo.it/copyright)



## License 

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) 

See [LICENSE](LICENSE) for full details.

    Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
    with the License.  You may obtain a copy of the License at

      https://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing,
    software distributed under the License is distributed on an
    "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.



## Trademarks

All other trademarks referenced herein are the property of their respective owners.



## NOTICE

This product includes software developed by
Cloud Posse, LLC (c) (https://cloudposse.com/)
Licensed under Apache License, Version 2.0
Copyright © 2017-2019 Cloud Posse, LLC
