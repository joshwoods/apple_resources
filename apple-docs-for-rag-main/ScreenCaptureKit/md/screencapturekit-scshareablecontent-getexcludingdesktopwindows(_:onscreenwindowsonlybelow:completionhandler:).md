

- ScreenCaptureKit
- SCShareableContent
-  getExcludingDesktopWindows(\_:onScreenWindowsOnlyBelow:completionHandler:) 

Type Method

# getExcludingDesktopWindows(\_:onScreenWindowsOnlyBelow:completionHandler:)

Retrieves the displays, apps, and windows that are behind the specified window.

Mac Catalyst 18.2+macOS 12.3+

``` source
class func getExcludingDesktopWindows(
    _ excludeDesktopWindows: Bool,
    onScreenWindowsOnlyBelow window: SCWindow,
    completionHandler: @escaping (SCShareableContent?, (any Error)?) -> Void
)
```

``` source
class func excludingDesktopWindows(
    _ excludeDesktopWindows: Bool,
    onScreenWindowsOnlyBelow window: SCWindow
) async throws -> SCShareableContent
```

## Parameters 

`excludeDesktopWindows`  

A Boolean value that indicates whether to exclude desktop windows from the set of shareable content.

`window`  

The window above which to retrieve shareable content.

`completionHandler`  

A callback the system invokes with the shareable content, or an error if a failure occurs.

## Discussion

Use this method to retrieve the onscreen content matching your filtering criteria. If the call is successful, the system passes an SCShareableContent instance to the completion handler; otherwise, it returns an error that describes the failure.

## See Also

### Retrieving shareable content

class func getWithCompletionHandler((SCShareableContent?, (any Error)?) -> Void)

Retrieves the displays, apps, and windows that your app can capture.

class func getExcludingDesktopWindows(Bool, onScreenWindowsOnly: Bool, completionHandler: (SCShareableContent?, (any Error)?) -> Void)

Retrieves the displays, apps, and windows that match your criteria.

class func getExcludingDesktopWindows(Bool, onScreenWindowsOnlyAbove: SCWindow, completionHandler: (SCShareableContent?, (any Error)?) -> Void)

Retrieves the displays, apps, and windows that are in front of the specified window.

class func info(for: SCContentFilter) -> SCShareableContentInfo

Retrieves any available sharable content information that matches the provided filter.

