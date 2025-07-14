

- ScreenCaptureKit
- SCShareableContent
-  getWithCompletionHandler(\_:) 

Type Method

# getWithCompletionHandler(\_:)

Retrieves the displays, apps, and windows that your app can capture.

Mac Catalyst 18.2+macOS 12.3+

``` source
class func getWithCompletionHandler(_ completionHandler: @escaping (SCShareableContent?, (any Error)?) -> Void)
```

``` source
class var current: SCShareableContent { get async throws }
```

## Parameters 

`completionHandler`  

A callback the system invokes with the shareable content, or an error if a failure occurs.

## Discussion

Use this method to retrieve the onscreen content that your app can capture. If the call is successful, the system returns the shareable content to the completion handler; otherwise, it returns an error that describes the failure.

## See Also

### Retrieving shareable content

class func getExcludingDesktopWindows(Bool, onScreenWindowsOnly: Bool, completionHandler: (SCShareableContent?, (any Error)?) -> Void)

Retrieves the displays, apps, and windows that match your criteria.

class func getExcludingDesktopWindows(Bool, onScreenWindowsOnlyAbove: SCWindow, completionHandler: (SCShareableContent?, (any Error)?) -> Void)

Retrieves the displays, apps, and windows that are in front of the specified window.

class func getExcludingDesktopWindows(Bool, onScreenWindowsOnlyBelow: SCWindow, completionHandler: (SCShareableContent?, (any Error)?) -> Void)

Retrieves the displays, apps, and windows that are behind the specified window.

class func info(for: SCContentFilter) -> SCShareableContentInfo

Retrieves any available sharable content information that matches the provided filter.

