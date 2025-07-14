

- Video Subscriber Account
-  VSAccountManagerDelegate 

Protocol

# VSAccountManagerDelegate

The methods you use to respond to authentication view controller requests.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
protocol VSAccountManagerDelegate : NSObjectProtocol
```

## Overview

Use the VSAccountManagerDelegate methods to aid in displaying and dismissing authentication view controllers.

If the user isn’t authenticated when your app calls enqueue(_:completionHandler:) with isInterruptionAllowed set to true, the system sends an authentication view controller to the delegate in the accountManager(_:present:) method for your app to present to the user.

## Topics

### Displaying Authentication Views

func accountManager(VSAccountManager, present: UIViewController)

Tells the delegate to present an authentication view controller.

**Required**

### Dismissing Authentication Views

func accountManager(VSAccountManager, dismiss: UIViewController)

Tells the delegate to dismiss an authentication view controller.

**Required**

### Supporting Degradation Scenarios

func accountManager(VSAccountManager, shouldAuthenticateAccountProviderWithIdentifier: String) -> Bool

Asks the delegate whether to authenticate the user with the selected provider.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to Account Manager Requests

var delegate: (any VSAccountManagerDelegate)?

The delegate of the account manager object.

