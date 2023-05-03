<!--
#
# Licensed to the Apache Software Foundation (ASF) under one
# or more contributor license agreements.  See the NOTICE file
# distributed with this work for additional information
# regarding copyright ownership.  The ASF licenses this file
# to you under the Apache License, Version 2.0 (the
# "License"); you may not use this file except in compliance
# with the License.  You may obtain a copy of the License at
#
# http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing,
# software distributed under the License is distributed on an
# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
#  KIND, either express or implied.  See the License for the
# specific language governing permissions and limitations
# under the License.
#
-->

# Newtmgr

Newt Manager (newtmgr) is the application tool that enables a user to communicate with and manage
remote devices running the Mynewt OS or Mcuboot.

### Building

1. `cd newtmgr`
2. `GO111MODULE=on go build`

### Usage

Upload app image
`./newtmgr --conntype serial --connstring $SERIAL_PORT,mtu=2048 image upload $PATH_TO_APP_BINARY`

Upload netcore image
`./newtmgr --conntype serial --connstring $SERIAL_PORT,mtu=2048 image upload $PATH_TO_NET_BINARY -n 3`
