

- App Intents
- ShortcutsLink
-  id(\_:) 

Instance Method

# id(\_:)

Binds a view’s identity to the given proxy value.

AppIntentsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func id(_ id: ID) -> some View where ID : Hashable
```

## Discussion

When the proxy value specified by the `id` parameter changes, the identity of the view — for example, its state — is reset.

