

- UIKit
- UIApplication
-  protectedDataDidBecomeAvailableNotification 

Type Property

# protectedDataDidBecomeAvailableNotification

A notification that posts when the protected files become available for your code to access.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
nonisolated
class let protectedDataDidBecomeAvailableNotification: NSNotification.Name
```

## Discussion

This notification does not contain a `userInfo` dictionary.

## See Also

### Accessing protected content

var isProtectedDataAvailable: Bool

A Boolean value that indicates whether content protection is active.

class let protectedDataWillBecomeUnavailableNotification: NSNotification.Name

A notification that posts shortly before protected files are locked down and become inaccessible.

