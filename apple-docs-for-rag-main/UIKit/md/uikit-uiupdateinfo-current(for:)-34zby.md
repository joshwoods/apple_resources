

- UIKit
- UIUpdateInfo
-  current(for:) 

Type Method

# current(for:)

Returns an object that describes the current UI update state for the specified view.

iOS 18.0+iPadOS 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
class func current(for view: UIView) -> Self?
```

## See Also

### Getting the current UI update information

class func current(for: UIWindowScene) -> Self?

Returns an object that describes the current UI update state for the specified window.

