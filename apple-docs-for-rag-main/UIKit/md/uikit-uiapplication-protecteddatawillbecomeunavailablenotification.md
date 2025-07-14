

- UIKit
- UIApplication
-  protectedDataWillBecomeUnavailableNotification 

Type Property

# protectedDataWillBecomeUnavailableNotification

A notification that posts shortly before protected files are locked down and become inaccessible.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
nonisolated
class let protectedDataWillBecomeUnavailableNotification: NSNotification.Name
```

## Discussion

Upon receiving this notification, clients should release any references to protected files. This notification does not contain a `userInfo` dictionary.

## See Also

### Accessing protected content

var isProtectedDataAvailable: Bool

A Boolean value that indicates whether content protection is active.

class let protectedDataDidBecomeAvailableNotification: NSNotification.Name

A notification that posts when the protected files become available for your code to access.

