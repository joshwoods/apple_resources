

- Technotes
-  TN3162: Understanding CloudKit throttles 

Article

# TN3162: Understanding CloudKit throttles

Learn how to identify and handle CloudKit throttles.

## Overview

The CloudKit infrastructure is shared by all apps and services. The resources are finite, and so high utilization from one app can negatively affect others. To avoid this kind of impact and optimize the overall experience, CloudKit implements a number of limits and controls on incoming traffic, which are known as *throttles*.

CloudKit can enforce throttles when it deems necessary on any app or service that uses the CloudKit framework, CloudKit Web Services, CloudKit JS, NSPersistentCloudKitContainer, and NSUbiquitousKeyValueStore. This technote discusses how to identify CloudKit throttles with representative error messages and how to handle them.

## Identify CloudKit throttles

The CloudKit server throttles a request from an app in the following cases:

- The app issues many CloudKit requests in a short time frame, and hits the rate limit.

- The app uses CloudKit in an inappropriate pattern, such as simultaneously triggering recurring spikes in request rates from many devices.

When the CloudKit server enforces throttles, it returns an error with a `retryAfter` value, which indicates how long the app should wait before retrying the request. For apps that use the CloudKit framework, the error is converted to .serviceUnavailable, with information shown in the following example:

```
[
    "CKErrorShouldThrottleClient": 1, 
    "RequestUUID": B59F1738-B330-4F27-A2AE-3C95572BC9F4, 
    "NSLocalizedDescription": Request failed with http status code 503, 
    "CKRetryAfter": 30, 
    "CKErrorDescription": Request failed with http status code 503, 
    "NSDebugDescription": CKInternalErrorDomain: 2022, 
    "NSUnderlyingError": 
]
```

For apps that use CloudKit Web Services or CloudKit JS, the error is conveyed in a server response with a body like the following example:

```
{
    "reason": "Database throttled, retry later",
    "retryAfter": 110207,
    "serverErrorCode": "THROTTLED",
    "error_code": "THROTTLED",
    "messageForDeveloper": "Database throttled, retry later",
    "uuid": wsThrottles_000029fa-7fd4-4eac-a5de-970942d10b7f
}
```

CloudKit on the device side can work with the server to enforce throttles as well. This prevents CloudKit requests from being sent to the server, and saves networking and server resources. When an app hits this kind of throttle, its CloudKit operation (CKOperation) gets a .requestRateLimited error, as shown in the following example:

```

```

Use these example messages to determine if your app hits CloudKit throttles. If you use the CloudKit framework, check if any CloudKit operation returns an `.serviceUnavailable` or `.requestRateLimited` error. For CloudKit Web Services or CloudKit JS, check if any response from the CloudKit server contains the `THROTTLED` error. Apps that use `NSPersistentCloudKitContainer` and `NSUbiquitousKeyValueStore` don’t perform CloudKit operations directly, so you need to look into a sysdiagnose. To capture and analyze a sysdiagnose, see Capture and analyze a sysdiagnose

Note

The system on a device can throttle CloudKit requests for other reasons. For example, when the battery level on an iPhone or Apple Watch runs low, iOS or watchOS may decide to defer a CloudKit operation, and this kind of throttle expires only after the battery returns to a high level. For more information, see Understand system throttles.

## Handle CloudKit throttles

CloudKit throttles are implemented to balance the use of CloudKit resources and achieve the best overall user experience of the service. When an app hits throttles, CloudKit stops accepting its requests until the throttles expire. There is no API for an app to configure the expiration time.

The best strategy to handle CloudKit throttles is to avoid them in the first place, and respect the `retryAfter` time if they happen. For apps that use the CloudKit framework, consider the following:

- Minimize the number of CloudKit operations and avoid doing many operations in a short time frame.

- Handle errors for every CloudKit operation. When hitting a `.requestRateLimited` or `.serviceUnavailable` error, retrieve the CKErrorRetryAfterKey value from the userInfo dictionary, and use it as the number of seconds to wait before retrying the operation.

- For operations that are not critical for the current launch session, schedule them as background tasks using the BackgroundTasks framework to have the system run the operations when it determines appropriate.

Note

Apps that use CKSyncEngine, which is a part of the CloudKit framework, don’t need to handle the errors. When hitting a throttle, `CKSyncEngine` respects it and automatically re-schedules the synchronization tasks after the `retry-after` time.

Similarly, apps that use CloudKit Web Services or CloudKit JS need to gracefully handle the throttle error the CloudKit server returns, and honor the `retry-after` time.

Apps that use `NSPersistentCloudKitContainer` and `NSUbiquitousKeyValueStore` automatically recover when the throttles expire. If they get throttled frequently, consider re-designing their architecture and workflow to avoid hitting the request rate limit.

A retried request is not guaranteed to succeed. It may be throttled again, with a new `retry-after` time, for the same reason. If your CloudKit requests keep getting throttled, even though your app doesn’t have a lot of CloudKit traffic, and the device, networking, and system status are all in a good state, consider providing your feedback.

## Revision History

- **2024-02-20** First published.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

TN3180: Reverting to App Store Server Notifications V1

Migrate from version 2 to version 1 of App Store Server Notifications using the Modify an App endpoint.

TN3179: Understanding local network privacy

Learn how local network privacy affects your software.

TN3178: Checking for and resolving build UUID problems

Ensure that every Mach-O image has a UUID, and that every distinct Mach-O image has its own unique UUID.

TN3177: Understanding alternate audio track groups in movie files

Learn how alternate groups collect audio tracks, and how to choose which audio track to use in your app.

TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

