

- SwiftUI
- NavigationLink
-  init(\_:value:) 

Initializer

# init(\_:value:)

Creates a navigation link that presents the view corresponding to a codable value, with a text label that the link generates from a localized string key.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    value: P?
) where Label == Text, P : Decodable, P : Encodable, P : Hashable
```

Available when `Label` conforms to `View` and `Destination` is `Never`.

Show all declarations

## Parameters 

`titleKey`  

A localized string that describes the view that this link presents.

`value`  

An optional value to present. When someone taps or clicks the link, SwiftUI stores a copy of the value. Pass a `nil` value to disable the link.

## Discussion

When someone activates the navigation link that this initializer creates, SwiftUI looks for a nearby navigationDestination(for:destination:) view modifier with a `data` input parameter that matches the type of this initializer’s `value` input, with one of the following outcomes:

- If SwiftUI finds a matching modifier within the view hierarchy of an enclosing NavigationStack, it pushes the modifier’s corresponding `destination` view onto the stack.

- If SwiftUI finds a matching modifier in the view hierarchy of a stack that’s in a later column of a NavigationSplitView, it puts the modifier’s destination view as the first and only item onto the stack while preserving the stack’s root view.

- If there’s no matching modifier, but the link appears in a List with selection inside a leading column of a navigation split view, the link updates the selection, which might affect the appearance of a trailing view. For an example of this, see NavigationLink.

- In other cases, the link doesn’t do anything.

Because this initializer takes a value that conforms to the Codable protocol, you ensure that a NavigationPath that includes this link can produce a non-`nil` value for its codable property. This helps to make the path serializable.

## See Also

### Presenting a value

init(value:label:)

Creates a navigation link that presents the view corresponding to a codable value.

