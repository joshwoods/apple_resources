

- SwiftUI
- Scene
-  environmentObject(\_:) 

Instance Method

# environmentObject(\_:)

Supplies an `ObservableObject` to a view subhierarchy.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func environmentObject(_ object: T) -> some Scene where T : ObservableObject
```

## Parameters 

`object`  

The object to store and make available to the scene’s subhierarchy.

## Discussion

The object can be read by any child by using `EnvironmentObject`:

```
final class Profile: ObservableObject { ... }

@main
struct MyApp: App {
    var body: some View {
        WindowGroup {
            ContentView()
        }
        .environment(ProfileService.currentProfile)
    }
}
```

You then read the object inside `ContentView` or one of its descendants using the EnvironmentObject property wrapper:

```
struct ContentView: View {
    @EnvironmentObject private var currentAccount: Account

    var body: some View { ... }
}
```

## See Also

### Distributing model data throughout your app

func environmentObject&lt;T>(T) -> some View

Supplies an observable object to a view’s hierarchy.

struct EnvironmentObject

A property wrapper type for an observable object that a parent or ancestor view supplies.

