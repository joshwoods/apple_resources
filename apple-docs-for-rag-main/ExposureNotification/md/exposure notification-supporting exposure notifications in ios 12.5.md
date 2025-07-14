

- Exposure Notification
-  Supporting Exposure Notifications in iOS 12.5 

Article

# Supporting Exposure Notifications in iOS 12.5

Prepare your Exposure Notifications app to run on a previous version of iOS.

## Overview

To increase adoption and broaden usage, the Exposure Notification framework now supports iPhones compatible with iOS 12.5. Because Exposure Notifications was originally released in iOS 13.5, special considerations apply when developing for iOS 12.5. However, all privacy protections put in place with the original release also apply in iOS 12.5.

### Determine the Level of Support You Need

Depending on your circumstances, you have a couple of options for adopting Exposure Notifications.

If you havenʼt already developed an Exposure Notifications app, or if you have an existing app that uses features in later versions of iOS that arenʼt available in iOS 12.5, consider using Exposure Notifications Express, which provides an app-less experience. For more information, see Supporting Exposure Notifications Express.

If you have an app that uses version 1 risk scoring and want to support iOS 12.5, consider updating to the more robust version 2 scoring. For more information, see ENExposureConfiguration.

### Set the Deployment Target and Link the Framework

Exposure Notifications for iOS 12.5 requires Xcode 12.3 or later. In your Xcode project’s Build Settings tab, set the iOS deployment target. From the menu, select Other and type “12.5.”

Select the Exposure Notification framework explicitly in the Link Binary With Libraries section under Build Phases. Set the status of the framework to Optional.

### Perform API and iOS Version Checks

Extend your app to handle different versions of iOS and Exposure Notifications by incorporating the following code. Call `getSupportedExposureNotificationsVersion()` to determine if Exposure Notifications is available on the device, and if so, which API version to support.

- Swift
- Objective-C

```
func ENManagerIsAvailable() -> Bool {
    return NSClassFromString("ENManager") != nil
}

enum SupportedENAPIVersion {
    case version2
    case version1
    case unsupported
}

func getSupportedExposureNotificationsVersion() -> SupportedENAPIVersion {
    if #available(iOS 13.7, *) {
        return .version2
    } else if #available(iOS 13.5, *) {
        return .version1
    } else if ENManagerIsAvailable() {
        return .version2
    } else {
        return .unsupported
    }
}
```

```
```

Although iOS 13.0 to 13.4 doesn’t support Exposure Notifications, your app might still download onto devices with those versions of iOS. If that happens, present a dialog to let the user know Exposure Notifications isn’t available for their device.

### Set Background Task Interval and Request Runtime

Apps that support Exposure Notifications periodically need time in the background to download and evaluate temporary exposure keys. Because BGTaskScheduler isn’t available in iOS 12.5, Bluetooth explicitly grants apps with the Exposure Notifications entitlement 3.5 minutes at least once a day.

Add the following code to your app to prepare it to receive background processing time at the defined interval.

- Swift
- Objective-C

```
struct ENActivityFlags: OptionSet {
    let rawValue: UInt32

    /// The app launched to perform periodic operations.
    static let periodicRun = ENActivityFlags(rawValue: 1  Void

extension ENManager {
    func setLaunchActivityHandler(activityHandler: @escaping ENActivityHandler) {
        let proxyActivityHandler: @convention(block) (UInt32) -> Void = {integerFlag in
            activityHandler(ENActivityFlags(rawValue: integerFlag))
        }       
        setValue(proxyActivityHandler, forKey: "activityHandler")
    }
 }
```

```
```

Background scheduling starts when the user authorizes and enables Exposure Notifications for the app. Upon user authorization, the first iteration of the background launch happens after the defined interval, and after every subsequent interval. If the app loses authorization, scheduling stops immediately.

Add the following code to your app to extend the `setLaunchActivityHandler` to download and detect exposures.

- Swift
- Objective-C

```
let manager = ENManager()

// Set the launch activity handler.
manager.setLaunchActivityHandler { activityFlags in
    if activityFlags.contains(.periodicRun) {
        // Your app now has 3.5 minutes to perform download and detection.
    }
}

// Activate the ENManager.
manager.activate { error in
    // Perform any error checking.
}

```

```
```

## See Also

### Essentials

Supporting Exposure Notifications Express

Configure servers to notify users of potential exposures to COVID-19 without an app.

Building an App to Notify Users of COVID-19 Exposure

Inform people when they may have been exposed to COVID-19.

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

