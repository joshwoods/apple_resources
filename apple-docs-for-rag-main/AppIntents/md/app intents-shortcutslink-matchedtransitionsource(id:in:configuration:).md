

- App Intents
- ShortcutsLink
-  matchedTransitionSource(id:in:configuration:) 

Instance Method

# matchedTransitionSource(id:in:configuration:)

Identifies this view as the source of a navigation transition, such as a zoom transition.

AppIntentsSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func matchedTransitionSource(
    id: some Hashable,
    in namespace: Namespace.ID,
    configuration: (EmptyMatchedTransitionSourceConfiguration) -> some MatchedTransitionSourceConfiguration
) -> some View
```

## Parameters 

`id`  

The identifier, often derived from the identifier of the data being displayed by the view.

`namespace`  

The namespace in which defines the `id`. New namespaces are created by adding an `Namespace` variable to a `View` type and reading its value in the view’s body method.

`configuration`  

A closure that you can use to apply styling to the source.

## Discussion

The appearance of the source can be configured using the `configuration` trailing closure. Any modifiers applied will be smoothly interpolated when a zoom transition originates from this matched transition source.

```
MyView()
    .matchedTransitionSource(id: someID, in: someNamespace) { source in
        source
            .cornerRadius(8.0)
    }
```

