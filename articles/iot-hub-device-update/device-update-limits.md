---
title: Understand Device Update for IoT Hub limits | Microsoft Docs
description: Key limits for Device Update for IoT Hub.
author: vimeht
ms.author: vimeht
ms.date: 9/9/2022
ms.topic: conceptual
ms.service: iot-hub-device-update
---

# Device Update for IoT Hub limits

This document provides an overview of the various limits that are imposed on the Device Update for IoT Hub resource and its associated operations. It also indicates whether the limits are adjustable by contacting Microsoft Support or not.

## Preview limits

During preview, the Device Update for IoT Hub service is provided at no cost to customers. More restrictive limits are imposed during the service's preview offering. These limits are expected to change once the service is generally available.

[!INCLUDE [device-update-for-iot-hub-limits](../../includes/device-update-for-iot-hub-limits.md)]

### Requirements for large-file downloads
If you plan to deploy large-file packages, with file size larger than 100 MB, it is recommended to utilize byte range requests for a reliable download performance.  

The Device Update for IoT Hub service utilizes Content Delivery Networks (CDNs) that work optimally with range requests of 1 MB in size. Range requests larger than 100 MB are not supported.

## Next steps

- [Create a Device Update for IoT Hub account](create-device-update-account.md)
- [Troubleshoot common Device Update for IoT Hub issues](troubleshoot-device-update.md)
