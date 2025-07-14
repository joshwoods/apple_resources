

- App Intents
- SiriTipView
-  environmentObject(\_:) 

Instance Method

# environmentObject(\_:)

Supplies an observable object to a view’s hierarchy.

AppIntentsSwiftUIiOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func environmentObject(_ object: T) -> some View where T : ObservableObject
```

## Parameters 

`object`  

The object to store and make available to the view’s hierarchy.

## Discussion

Use this modifier to add an observable object to a view’s environment. The object must conform to the ObservableObject protocol.

Adding an object to a view’s environment makes the object available to subviews in the view’s hierarchy. To retrieve the object in a subview, use the `EnvironmentObject` property wrapper.

Note

If the observable object conforms to the Observable protocol, use either `View/environment(_:)` or the `View/environment(_:_:)` modifier to add the object to the view’s environment.

