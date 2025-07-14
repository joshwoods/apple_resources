

- SwiftUI
- OpenURLAction
- OpenURLAction.Result
-  systemAction 

Type Property

# systemAction

The handler asks the system to open the original URL.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let systemAction: OpenURLAction.Result
```

## Discussion

The action invokes its completion handler with a value that depends on the outcome of the system’s attempt to open the URL.

## See Also

### Getting the results

static let discarded: OpenURLAction.Result

The handler discarded the URL.

static let handled: OpenURLAction.Result

The handler opened the URL.

static func systemAction(URL) -> OpenURLAction.Result

The handler asks the system to open the modified URL.

