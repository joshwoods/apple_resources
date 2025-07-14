

- UIKit
- UIApplication
-  isProtectedDataAvailable 

Instance Property

# isProtectedDataAvailable

A Boolean value that indicates whether content protection is active.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
nonisolated
var isProtectedDataAvailable: Bool { get }
```

## Discussion

The value of this property is false if data protection is enabled and the device is currently locked. The value of this property is set to true if the device is unlocked or if content protection is not enabled.

When the value of this property is false, files that were assigned the complete or completeUnlessOpen protection key cannot be read or written by your app. The user must unlock the device before your app can access them.

## See Also

### Accessing protected content

class let protectedDataDidBecomeAvailableNotification: NSNotification.Name

A notification that posts when the protected files become available for your code to access.

class let protectedDataWillBecomeUnavailableNotification: NSNotification.Name

A notification that posts shortly before protected files are locked down and become inaccessible.

