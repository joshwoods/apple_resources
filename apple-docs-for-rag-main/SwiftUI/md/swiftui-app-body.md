

- SwiftUI
- App
-  body 

Instance Property

# body

The content and behavior of the app.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@SceneBuilder @MainActor @preconcurrency
var body: Self.Body { get }
```

**Required**

## Discussion

For any app that you create, provide a computed `body` property that defines your app’s scenes, which are instances that conform to the Scene protocol. For example, you can create a simple app with a single scene containing a single view:

```
@main
struct MyApp: App {
    var body: some Scene {
        WindowGroup {
            Text("Hello, world!")
        }
    }
}
```

Swift infers the app’s Body associated type based on the scene provided by the `body` property.

## See Also

### Implementing an app

associatedtype Body : Scene

The type of scene representing the content of the app.

**Required**

