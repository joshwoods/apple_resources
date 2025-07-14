

- UIKit
- UIUpdateLink
-  currentUpdateInfo() 

Instance Method

# currentUpdateInfo()

Returns an object that describes the current UI update state.

iOS 18.0+iPadOS 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
func currentUpdateInfo() -> UIUpdateInfo?
```

## Return Value

During a UI update, returns a UIUpdateInfo object that describes the current UI update state. Outside a UI update, returns `nil`.

## See Also

### Getting the current UI update information

class UIUpdateInfo

An object that contains detailed information about the current UI update state.

