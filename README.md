# balena-node-red-watcher

![seeed-watcher-poster](https://github.com/user-attachments/assets/35c743d4-2863-4172-9e4b-b2efc1f80662)

A Node-RED application with [SenseCAP Watcher](https://wiki.seeedstudio.com/watcher/) flow [support](https://github.com/balena-io-projects/node-red-contrib-balena), can be managed remotely via balena [publicURL](https://balena.io/docs/learn/manage/actions/#enable-public-device-url)

You can deploy this project to a new balenaCloud application in one click using the button below:

[![](https://balena.io/deploy.svg)](https://dashboard.balena-cloud.com/deploy?repoUrl=https://github.com/balenalabs/balena-node-red)

Or, you can create an application in your balenaCloud dashboard and balena push this code to it the traditional way.

![mqdefault](https://github.com/user-attachments/assets/2d580019-2db8-4d36-869d-cf01848ed69d)

## Import the flow

After you deploy the app, enable public device url, then import the node-red flow thats comes with the deployment.

![import_flow_to_nodered](https://github.com/user-attachments/assets/ac2afe9e-03dd-43c2-ab8e-cd96fa0f41f0)

You need to get SenseCAP Organization ID and API key from [Sensecap Portal](https://sensecap.seeed.cc/portal/#/dashboard) -> Access API Keys

## Environment variables

| Variable Name  | Default  | Description                                             |
| -------------- | -------- | ------------------------------------------------------- |
| PORT           | `80`     | the port that exposes the Node-RED UI                   |
| USERNAME       | `balena` | the Node-RED admin username                             |
| PASSWORD       | `balena` | the Node-RED admin password                             |
| ENCRIPTION_KEY | `balena` | the encription key used to store your credentials files |

You **must** set the `USERNAME` and `PASSWORD` environment variables to be able to save or run programs in Node-RED.  
More information about using and setting environment variables can be found in
the [balena docs](https://balena.io/docs/learn/manage/serv-vars/).

## License

Copyright 2016 balena Ltd.

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

<http://www.apache.org/licenses/LICENSE-2.0>

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
