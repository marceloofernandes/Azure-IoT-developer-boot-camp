# Azure-IoT-developer-boot-camp

## Project name:
Azure IoT developer boot camp lab

### Description:
This hands-on lab is part of the IoT School learning path about Azure IoT solutions provided by Microsoft. Its goal is to ` "get started with Azure IoT. This is a series of hands-on labs for anyone who is learning about Azure Internet of Things (IoT). In these labs, you will use Azure services to build Azure IoT end-to-end solutions, connecting real and simulated devices to Azure IoT Hub." ` It is available at https://iotschool.microsoft.com/learning-paths/1z75cTRBNqEA2EigQoQKKe or https://github.com/Azure-Samples/azureiotlabs.

### 10 Modules:

Total duration: 7hr 33min

### Module 1: How to use the following hands-on labs?

Duration: 3 minutes

### Module 2: Introduction to Azure IoT Hub and connect MXChip.

Duration: 60 minutes

Instructions: https://azure-samples.github.io/azureiotlabs/IoTHub/

(This module requires the MXChip board)


### Module 3: Connect a Pi simulator to Azure IoT Hub
Duration: 30 minutes
Instructions: https://azure-samples.github.io/azureiotlabs/IoTHub-PiSimulator/
(paste results)

### Module 4: Visualize time-series data with Azure Time Series Insights
Duration: 60 minutes
Instructions: https://azure-samples.github.io/azureiotlabs/timeseriesinsights/

### Module 5: React to critical device lifecycle events and trigger Actions
Duration: 30 minutes
Instructions: https://azure-samples.github.io/azureiotlabs/EventGrid/

### Module 6: Cold path storage
Duration: 90 minutes
Instructions: https://azure-samples.github.io/azureiotlabs/DatalakeStore/
(incomplete)

### Module 7: Hot path analytics
Duration: 60 minutes
Instructions: https://azure-samples.github.io/azureiotlabs/CosmosDB/
(incomplete)

### Module 8: Batch analytics
Duration: 60 minutes
Instructions: https://azure-samples.github.io/azureiotlabs/DatalakeAnalytics/
(incomplete)

### Module 9: Load test using Device Simulator
Duration: 30 minutes
Instructions: https://azure-samples.github.io/azureiotlabs/DeviceSimulator/
Create Device Simulator: https://www.azureiotsolutions.com/Accelerators (the provided URL https://www.azureiotsuite.com/ was not working at the time of this lab)
PS: This activity needs to be updated. The instructions leads to differents windows (pictures)

### Module 10: Configure and monitor IoT devices at scale
Duration: 30 minutes
Instructions: https://github.com/Azure-Samples/azureiotlabs/blob/master/automaticdeviceconfiguration/README.md
PS: Paty attention to "Step 2: Specify Settings", there is a typo in JSON "74". It should 74.


Below is the device twin updated with properties:
```
{
  "deviceId": "shinagawahvac1",
  "etag": "AAAAAAAAAAQ=",
  "deviceEtag": "MTI5Mjg0NTg5",
  "status": "enabled",
  "statusUpdateTime": "0001-01-01T00:00:00",
  "connectionState": "Disconnected",
  "lastActivityTime": "0001-01-01T00:00:00",
  "cloudToDeviceMessageCount": 0,
  "authenticationType": "sas",
  "x509Thumbprint": {
    "primaryThumbprint": null,
    "secondaryThumbprint": null
  },
  "version": 5,
  "tags": {
    "location": {
      "city": "Shinagawa"
    }
  },
  "properties": {
    "desired": {
      "hvacsettings": {
        "temperature": 74,
        "humidity": 28
      },
      "$metadata": {
        "$lastUpdated": "2018-12-20T20:37:20.3275207Z",
        "$lastUpdatedVersion": 2,
        "hvacsettings": {
          "$lastUpdated": "2018-12-20T20:37:20.3275207Z",
          "$lastUpdatedVersion": 2,
          "temperature": {
            "$lastUpdated": "2018-12-20T20:37:20.3275207Z",
            "$lastUpdatedVersion": 2,
            "$lastUpdatedBy": "shinagawahvacsetting",
            "$lastUpdatedByDigest": "636809350366618253"
          },
          "humidity": {
            "$lastUpdated": "2018-12-20T20:37:20.3275207Z",
            "$lastUpdatedVersion": 2,
            "$lastUpdatedBy": "shinagawahvacsetting",
            "$lastUpdatedByDigest": "636809350366618253"
          }
        }
      },
      "$version": 2
    },
    "reported": {
      "$metadata": {
        "$lastUpdated": "2018-12-20T20:02:32.3175557Z"
      },
      "$version": 1
    }
  },
  "configurations": {
    "shinagawahvacsetting": {
      "status": "Applied"
    }
  },
  "capabilities": {
    "iotEdge": false
  }
}
```
