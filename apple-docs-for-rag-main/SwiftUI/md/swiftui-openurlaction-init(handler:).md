

- SwiftUI
- OpenURLAction
-  init(handler:) 

Initializer

# init(handler:)

Creates an action that opens a URL.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@MainActor @preconcurrency
init(handler: @escaping (URL) -> OpenURLAction.Result)
```

## Parameters 

`handler`  

The closure to run for the given URL. The closure takes a URL as input, and returns a OpenURLAction.Result that indicates the outcome of the action.

## Discussion

Use this initializer to create a custom action for opening URLs. Provide a handler that takes a URL and returns an OpenURLAction.Result. Place your handler in the environment using the environment(_:_:) view modifier:

```
Text("Visit [Example Company](https://www.example.com) for details.")
    .environment(\.openURL, OpenURLAction { url in
        handleURL(url) // Define this method to take appropriate action.
        return .handled
    })
```

Any views that read the action from the environment, including the built-in Link view and Text views with markdown links, or links in attributed strings, use your action.

SwiftUI translates the value that your custom action’s handler returns into an appropriate Boolean result for the action call. For example, a view that uses the action declared above receives `true` when calling the action, because the handler always returns handled.

## See Also

### Creating the action

struct Result

The result of a custom open URL action.

