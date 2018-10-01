arm PELION Device Shadow bridge for Microsoft IoTHub                  
  
09/30/2018: updated properties-editor - update POST methods

09/30/2018: updated bridge - added JVM memory statistics

09/29/2018: updated bridge - fixes and updates 

09/28/2018: synced update

09/28/2018: updated bridge and properties-editor - fixes for VM installations 

09/27/2018: updated bridge - better support for non-MQTT peer interfaces

09/26/2018: synced update

09/20/2018: updated bridge - misc sync

09/19/2018: updated bridge - misc sync

09/17/2018: updated bridge - misc sync

09/14/2018: updated bridge - Google OBS and Null Pointer fixes

09/13/2018: synced update

09/10/2018: updated bridge - Watson IoT fixes

09/10/2018: resynced with templated add-on sample

09/09/2018: updated bridge - misc syncs 

09/06/2018: updated bridge - more cleanup and removal of older subscription management. Webhook reset finished. 

Container Bridge Instance Installation:

1). Clone this repo into a Linux instance that supports docker images

2). cd into the cloned repo and run: ./run-reload-bridge.sh

Once the container instance is live, you must configure the bridge and bind it between your mbed Pelion account and your IoTHub Account in Azure. 

1). Please go to your Azure dashboard and create an IoTHub instance.

2). From your IoTHub dashboard in Azure, copy to your clipboard your IoTHub's "iothubowner" primary key connection string. Record the connection string.

3). Next go to https://os.mbed.com and create your mbed Account. You can then request a Pelion developer account using the same credentials at https://portal.us-east-1.mbedcloud.com

4). Once your Pelion account is created, you need to "Access Keys" to create a Pelion API Key/Token. Record the Token Value

Now that you have your:

    - IoTHub "iothubowner" primary key connection string

    - Pelion API Key/Token generated

Go to:  https://[[your containers public IP address]]:8234

    - username: "admin" (no quotes)

    - password: "admin" (no quotes)

Enter both your IoTHub "iothubowner" connection string and the Pelion API Token

    - Please press "SAVE" after *each* is entered... 

    - After both are entered and saved, press "RESTART"

Your Pelion bridge should now be configured and operational. 

Bridge source (Apache 2.0 licensed - Enjoy!): https://github.com/ARMmbed/pelion-bridge.git

Copyright 2018. ARM Ltd. All rights reserved.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License. 
