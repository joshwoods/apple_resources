

- Exposure Notification
-  Building an App to Notify Users of COVID-19 Exposure 

Sample Code

# Building an App to Notify Users of COVID-19 Exposure

Inform people when they may have been exposed to COVID-19.

Download

iOS 12.5+iPadOS 12.5+Xcode 12.4+

## Overview

This code project uses the Exposure Notification framework to build a sample app that demonstrates how to notify people when they have come into contact with someone who meets a set of criteria for a case of COVID-19. When using the project as a reference for designing an Exposure Notifications app, you can define the criteria for how the framework determines whether the risk is high enough to report to the user.

The sample app includes code to simulate server responses. When building an Exposure Notifications app based on this project, create a server environment to provide diagnosis keys and exposure criteria, and add code to your app to communicate with this server. If the app you build operates in a country that authenticates medical tests for COVID-19, you may need to include additional network code to communicate with those authentication services.

Exposure Notifications is available on all iOS devices running iOS 13.5 or later. It’s also available on iOS 12.5 with some additional setup. The Xcode project has two targets:

- ExposureNotificationApp — Supports iOS 13.5 and later

- ExposureNotificationApp-iOS12 — Supports iOS 12.5, and iOS 13.5 and later

For more information on the architecture and security of the Exposure Notification service, see Privacy-Preserving Contact Tracing. For more information on supporting iOS 12.5 in your Exposure Notifications App, see Supporting Exposure Notifications in iOS 12.5.

### Configure the Sample Code Project

Before you run the sample code project in Xcode, make sure:

- Your iOS device is running either iOS 12.5 or 13.5 or later.

- You are running Xcode 12 or later.

- You configure the project with a provisioning profile that includes the Exposure Notification entitlement. To get permission to use this entitlement, see Exposure Notification Entitlement Request.

### Authorize Exposure Notifications

Users must explicitly authorize an app to use Exposure Notifications. The ENManager class provides information on the user’s authorization status and requests authorization. The project has a singleton class called `ExposureManager` that instantiates and manages the life cycle of an `ENManager` object. During `init`, It calls activate(completionHandler:) on `ENManager`, then checks the callback to find out if Exposure Notifications is enabled. If it isn’t, `ExposureManager` attempts to enable it.

```
```

### Store User Data Locally

The app stores information about test results and high-risk exposures in the user defaults directory. The local data is private and stays on the device.

A custom property wrapper transforms data between its native format and a JSON-formatted equivalent, reads and writes data in the user defaults dictionary, and posts notifications to the app when local data changes. The `LocalStore` class manages the user’s private data, defined as a series of properties that all use this property wrapper.

```
```

The app defines its own data structures for any data it persists. For example, a test result records the date the user took the test, and whether the user shared this data with the server. This information is used to populate the user interface.

```
```

### Share Diagnosis Keys with the Server

A user with a diagnosis for COVID-19 can upload *diagnosis keys* to the server. Each instance of the app periodically downloads diagnosis keys to search the device’s private interaction data for matching interactions.

This project simulates a remote server with which the app communicates. There is a single `Server` object in the app that stores the received diagnosis keys and provides them on demand. The sample server does not partition the data by region. It maintains a single list of keys, and provides the entire list upon request.

```
```

As with the local store, this local server stores the data in JSON format, using the same `Persisted` property wrapper.

### Ask Users to Share COVID-19 Indicators

The sample app demonstrates a strategy in which a recognized medical authority tested the user and found positive COVID-19 indicators. The sample app provides a way for users to enter an authentication code, but doesn’t submit this data to an authentication service, so all codes automatically pass.

When the user provides information about a positive test result, the app records the test result in the local store and asks the user to share it. To share the result, the app needs to get a list of diagnosis keys and send the list to the server. To get the keys, the app calls the singleton `ENManager` object’s getDiagnosisKeys(completionHandler:) method, as shown in the code below.

```
```

Each time the app calls this method, the user must authorize the transaction. The framework then returns the list of keys to the app. The app sends those keys as-is to the server and then updates the test record to indicate that it was shared.

The sample app’s server implementation appends the keys onto a list it maintains, skipping any keys that are already there. It stores the keys sequentially so that the app can request just the keys it hasn’t received before.

```
```

### Ask Users to Preauthorize Key Release at the Time of the Test

Starting with iOS 14.4, the Exposure Notification framework allows apps to ask users for permission to release temporary exposure keys when they take a COVID-19 diagnostic test. This authorization lasts for up to five days and should be requested only if the app determines that the user is about to take a test and the app has a way to determine the results. To request preauthorization, the app calls preAuthorizeDiagnosisKeys(completionHandler:).

```
```

Within five days of being granted permission, if the app determines that the user has received a positive test result, it can request the preauthorized keys and submit them to the key server. `ENManager` sends keys to the app using a completion handler property called diagnosisKeysAvailableHandler, which the app sets before requesting the keys:

```
```

After setting the `diagnosisKeysAvailableHandler` property, the app requests the keys by calling requestPreAuthorizedDiagnosisKeys(completionHandler:). This call returns an error if the user doesn’t authorize release or if more than five days pass after authorization. Otherwise, the completion handler is called with the keys. When the sample app releases the keys, it notifies the user that because they’ve had a positive test result, their keys are being shared pursuant to their prior authorization.

```
```

Important

PHAs must notify users that they’ve tested positive *before* the app calls `requestPreAuthorizedDiagnosisKeys(completionHandler:)`. They must also notify users that their keys are being submitted to the PHA’s key server.

### Detect Exposure Notifications API Version at Runtime

The Exposure Notifications APIs are available in the following distinct versions that implement slightly different versions of the detection algorithm:

- Version 1 — Devices running iOS 13.5 or iOS 13.6 support the version 1 API only. To prevent runtime errors, Exposure Notifications apps for iOS 13.5 and iOS 13.6 must fall back to this version.

- Version 2 — When available, apps should use this version of the API.

The sample app includes a utility function to determine which API versions are available on the current device:

```
```

The main difference between using the two API versions is the method called to detect exposures. When running on devices that only support version 1, the sample app uses getExposureInfo(summary:userExplanation:) to evaluate diagnosis keys for potential exposures. When running on devices that support version 2 of the API, it uses getExposureWIndows(summary:completionHandler:) instead.

```
```

### Check for Exposures in iOS 13.5+

The ExposureNotificationApp target demonstrates how to create a background task in iOS 13.5 or later to periodically download new keys and check whether the user may have been exposed to an individual with COVID-19.

The app’s `Info.plist` file declares a background task named `com.example.apple-samplecode.ExposureNotificationSampleApp.exposure-notification`. The Background Task framework automatically detects apps that contain the Exposure Notification entitlement and a background task that ends in `exposure-notification`. The operating system automatically launches these apps when they aren’t running and guarantees them more background time to ensure that the app can test and report results promptly.

```
```

First, the background task provides a handler in case it runs out of time. Then it calls the app’s `detectExposures` method to test for exposures. Finally, it schedules the next time the system should execute the background task.

```
```

### Check for Exposures in iOS 12.5

To support iOS 12.5, apps must register an activity handler with `ENManager`’s `setLaunchActivityHandler()` instead of creating a background task, but only when running on iOS 12.5. This step is necessary because Background Tasks do not exist in iOS 12.5. Instead, `ENManager` provides apps that register an activity handler with 3.5 minutes of background processing at least once per day.

```
```

The remaining sections describe how the app obtains the set of diagnosis keys and submits them to the framework for evaluation.

### Download Diagnosis Keys

The app downloads diagnosis keys from the server to pass to the framework, starting with the first key the app hasn’t downloaded before. This design ensures that the app checks each diagnosis key only once on any given device.

The app needs to provide signed key files to the framework. The app asks the server for the URLs of any key files that the server generated after the last file that the app checked. After receiving the URLs from the server, the app uses a dispatch group to download the files to the device.

```
```

Finally, the app creates an array of the local URLs for the downloaded files.

```
```

### Configure Criteria to Estimate Risk

The framework will compare locally saved interaction data against the diagnosis keys provided by the app. When the framework finds a match, it calculates a risk score for that interaction based on a number of different factors, such as when the interaction took place and how long the devices were in proximity to each other.

To provide specific guidance to the framework about how risk should be evaluated, the app creates an ENExposureConfiguration object. The app requests the criteria from the `Server` object, which creates and returns an `ENExposureConfiguration` object as shown below. The sample configuration has placeholder data that evaluates any interaction as risky, so the framework returns all interactions that match the diagnosis keys.

```
```

### Submit Diagnosis Keys to the Framework

After downloading the key files, the app performs the search for exposures using a series of asynchronous steps. First, the app requests the criteria from the server, which calls into the code shown in the Configure Criteria to Estimate Risk section above. Then the app calls the `ENManager` objects’s detectExposures(configuration:diagnosisKeyURLs:completionHandler:) method, passing the criteria and the URLs for the downloaded key files. This method returns a summary of the search results.

The code then passes off the downloaded keys to one of two different methods based on which API version is available on the device.

```
```

Finally, the app calls its `finish` method to complete the search. The `finish` method updates the local store with the new data, including any exposures, the date and time the app executed the search, and the index for the key file to check next time.

## See Also

### Essentials

Supporting Exposure Notifications Express

Configure servers to notify users of potential exposures to COVID-19 without an app.

Setting Up a Key Server

Ensure that your server meets the requirements for supporting Exposure Notifications.

class ENManager

A class that manages exposure notifications.

ENDeveloperRegion

A string that specifies the region that the app supports.

ENAPIVersion

A number that specifies the version of the API to use.

Changing Configuration Values Using the Server‑to‑Server API

Update Exposure Notifications configuration values from a Public Health Authority’s server.

Testing Exposure Notifications Apps in iOS 13.7 and Later

Perform end-to-end validation of Exposure Notifications apps on a device by manually loading configuration files.

Supporting Exposure Notifications in iOS 12.5

Prepare your Exposure Notifications app to run on a previous version of iOS.

