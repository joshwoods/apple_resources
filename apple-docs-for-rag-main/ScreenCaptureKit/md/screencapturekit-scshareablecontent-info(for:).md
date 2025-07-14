

- ScreenCaptureKit
- SCShareableContent
-  info(for:) 

Type Method

# info(for:)

Retrieves any available sharable content information that matches the provided filter.

Mac Catalyst 17.0+macOS 14.0+

``` source
class func info(for filter: SCContentFilter) -> SCShareableContentInfo
```

## Parameters 

`filter`  

The filter to match current sharable content against.

## Return Value

The sharable content matching the filter, or `nil` if none is found.

## See Also

### Retrieving shareable content

class func getWithCompletionHandler((SCShareableContent?, (any Error)?) -> Void)

Retrieves the displays, apps, and windows that your app can capture.

class func getExcludingDesktopWindows(Bool, onScreenWindowsOnly: Bool, completionHandler: (SCShareableContent?, (any Error)?) -> Void)

Retrieves the displays, apps, and windows that match your criteria.

class func getExcludingDesktopWindows(Bool, onScreenWindowsOnlyAbove: SCWindow, completionHandler: (SCShareableContent?, (any Error)?) -> Void)

Retrieves the displays, apps, and windows that are in front of the specified window.

class func getExcludingDesktopWindows(Bool, onScreenWindowsOnlyBelow: SCWindow, completionHandler: (SCShareableContent?, (any Error)?) -> Void)

Retrieves the displays, apps, and windows that are behind the specified window.

