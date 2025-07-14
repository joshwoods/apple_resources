

- SwiftUI
- OpenURLAction
- OpenURLAction.Result
-  handled 

Type Property

# handled

The handler opened the URL.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let handled: OpenURLAction.Result
```

## Discussion

The action invokes its completion handler with `true` when your handler returns this value.

## See Also

### Getting the results

static let discarded: OpenURLAction.Result

The handler discarded the URL.

static let systemAction: OpenURLAction.Result

The handler asks the system to open the original URL.

static func systemAction(URL) -> OpenURLAction.Result

The handler asks the system to open the modified URL.

