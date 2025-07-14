

- Exposure Notification
-  ENManager 

Class

# ENManager

A class that manages exposure notifications.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
class ENManager
```

## Overview

Important

This class is available in iOS 12.5, and in iOS 13.5 and later.

Before using an instance of this class, call activate(completionHandler:). If the completion handler completes successfully, you can work with the remaining properties and methods on the class. Activating this object doesn’t enable exposure notification; it only allows this object to be used. Once activated, exposure notification can be enabled with setExposureNotificationEnabled(_:completionHandler:), if needed.

If the app no longer needs an instance of this class, you must call invalidate(), which stops any outstanding operations and invokes the invalidation handler.

Note

Invalidation is asynchronous so it’s possible for handlers to be invoked after calling invalidate().

The framework invokes the invalidation handler once invalidation finishes, and performs the invocation exactly once, even if invalidate() is called multiple times. It does not call any additional handlers.

After calling invalidate(), your app can’t reuse the object. A new object must be created for subsequent use. The framework clears strong references once invalidation completes to break potential retain cycles. You don’t need to use weak references within your handlers to avoid retain cycles when using this class.

## Topics

### Activating the Manager

func activate(completionHandler: ENErrorHandler)

Prepares the manager for use.

var activityHandler: ENActivityHandler?

The handler that the framework invokes when the app activates a notification manager.

typealias ENActivityHandler

The handler the system invokes to report activities that occurred while the app wasn’t running.

struct ENActivityFlags

Activities that occur while the app isn’t running.

func setExposureNotificationEnabled(Bool, completionHandler: ENErrorHandler)

Enables or disables exposure notification.

### Obtaining Exposure Information

func detectExposures(configuration: ENExposureConfiguration, diagnosisKeyURLs: [URL], completionHandler: ENDetectExposuresHandler) -> Progress

Detects exposures using the configuration that you specify for controlling the scoring algorithm.

func detectExposures(configuration: ENExposureConfiguration, completionHandler: ENDetectExposuresHandler) -> Progress

Detects exposures using the specified configuration to control the scoring algorithm.

func getExposureWindows(summary: ENExposureDetectionSummary, completionHandler: ENGetExposureWindowsHandler) -> Progress

Obtains information from the provided summary about the user’s exposure within a window of time.

typealias ENGetExposureWindowsHandler

The handler the system invokes when the acquisition of windows completes.

func getUserTraveled(completionHandler: ENGetUserTraveledHandler)

Obtains information about the user’s travel within an exposure period.

typealias ENGetUserTraveledHandler

The handler the system invokes when acquistiion of the user’s travel status completes.

func getExposureInfo(summary: ENExposureDetectionSummary, userExplanation: String, completionHandler: ENGetExposureInfoHandler) -> Progress

Returns information about each exposure.

Deprecated

### Obtaining Exposure Keys

func getDiagnosisKeys(completionHandler: ENGetDiagnosisKeysHandler)

Requests the temporary exposure keys from the user’s device to share with a server.

func getTestDiagnosisKeys(completionHandler: ENGetDiagnosisKeysHandler)

Requests the temporary exposure keys, including the current key, used by this device for testing.

class ENTemporaryExposureKey

The key used to generate rolling proximity identifiers.

### Configuring the Manager

var exposureNotificationStatus: ENStatus

A property that indicates the status of exposure notifications.

var exposureNotificationEnabled: Bool

A property that indicates that a user enabled exposure notification.

class var authorizationStatus: ENAuthorizationStatus

A property that reports the current authorization status of the app, and never prompts the user.

var dispatchQueue: dispatch_queue_t

The dispatch queue on which to invoke handlers.

### Preauthorizing Exposure Keys

func requestPreAuthorizedDiagnosisKeys(completionHandler: ENErrorHandler)

Requests diagnosis keys after the user authorizes sharing them.

func preAuthorizeDiagnosisKeys(completionHandler: ENErrorHandler)

Allows users to authorize a one-time release of diagnosis keys within five days of the authorization.

typealias ENDiagnosisKeysAvailableHandler

The handler the system invokes after requesting diagnosis keys.

var diagnosisKeysAvailableHandler: ENDiagnosisKeysAvailableHandler?

The handler that receives available diagnosis keys after a successful preauthorization.

### Invalidating the Manager

func invalidate()

Stops any outstanding operations and invalidates the manager.

### Instance Properties

var invalidationHandler: (() -> Void)?

The handler that the framework invokes when invalidation completes.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Essentials

Supporting Exposure Notifications Express

Configure servers to notify users of potential exposures to COVID-19 without an app.

Building an App to Notify Users of COVID-19 Exposure

Inform people when they may have been exposed to COVID-19.

Setting Up a Key Server

Ensure that your server meets the requirements for supporting Exposure Notifications.

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

