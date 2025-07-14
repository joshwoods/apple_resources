

- App Intents
- ShortcutsLink
-  accessibilityElement(children:) 

Instance Method

# accessibilityElement(children:)

Creates a new accessibility element, or modifies the `AccessibilityChildBehavior` of the existing accessibility element.

AppIntentsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func accessibilityElement(children: AccessibilityChildBehavior = .ignore) -> some View
```

## Parameters 

`children`  

The behavior to use when creating or transforming an accessibility element. The default is `AccessibilityChildBehavior/ignore`

## Discussion

See also:

- `AccessibilityChildBehavior/ignore`

- `AccessibilityChildBehavior/combine`

- `AccessibilityChildBehavior/contain`

