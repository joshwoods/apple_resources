

- SwiftUI
- OpenURLAction
-  OpenURLAction.Result 

Structure

# OpenURLAction.Result

The result of a custom open URL action.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Result
```

## Overview

If you declare a custom OpenURLAction in the Environment, return one of the result values from its handler.

- Use handled to indicate that the handler opened the URL.

- Use discarded to indicate that the handler discarded the URL.

- Use systemAction without an argument to ask SwiftUI to open the URL with the system handler.

- Use systemAction(_:) with a URL argument to ask SwiftUI to open the specified URL with the system handler.

You can use the last option to transform URLs, while still relying on the system to open the URL. For example, you could append a path component to every URL:

```
.environment(\.openURL, OpenURLAction { url in
    .systemAction(url.appendingPathComponent("edit"))
})
```

## Topics

### Getting the results

static let discarded: OpenURLAction.Result

The handler discarded the URL.

static let handled: OpenURLAction.Result

The handler opened the URL.

static let systemAction: OpenURLAction.Result

The handler asks the system to open the original URL.

static func systemAction(URL) -> OpenURLAction.Result

The handler asks the system to open the modified URL.

## Relationships

### Conforms To

- Sendable

## See Also

### Creating the action

init(handler: (URL) -> OpenURLAction.Result)

Creates an action that opens a URL.

