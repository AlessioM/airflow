<!--
 Licensed to the Apache Software Foundation (ASF) under one
 or more contributor license agreements.  See the NOTICE file
 distributed with this work for additional information
 regarding copyright ownership.  The ASF licenses this file
 to you under the Apache License, Version 2.0 (the
 "License"); you may not use this file except in compliance
 with the License.  You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

 Unless required by applicable law or agreed to in writing,
 software distributed under the License is distributed on an
 "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 KIND, either express or implied.  See the License for the
 specific language governing permissions and limitations
 under the License.
 -->

## Release 2021.2.5

### Bug fixes

  * `Remove failed DockerOperator tasks with auto_remove=True (#13532) (#13993)`
  * `Fix error on DockerSwarmOperator with auto_remove True (#13532) (#13852)`
### Changes to XCom return values

* the return value of XCom is of type `str` (as opposed to `bytes`)
* if `xcom_all` is set to `False` only the last line of the log (separated by `\n`) will be included in the XCom value
