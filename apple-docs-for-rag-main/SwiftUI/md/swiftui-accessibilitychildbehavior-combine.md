

- SwiftUI
- AccessibilityChildBehavior
-  combine 

Type Property

# combine

Any child accessibility element’s properties are merged into the new accessibility element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let combine: AccessibilityChildBehavior
```

## Discussion

Use this behavior when you want a view represented by a single accessibility element. The new accessibility element merges properties from all non-hidden children. Some properties may be transformed or ignored to achieve the ideal combined result. For example, not all of AccessibilityTraits are merged and a default action may become a named action (init(named:)).

```
struct UserCell: View {
    var user: User

    var body: some View {
        VStack {
            Image(user.image)
            Text(user.name)
            Button("Options", action: showOptions)
        }
        .accessibilityElement(children: .combine)
    }
}
```

A new accessibility element is created when:

- The view contains multiple or zero accessibility elements

- The view wraps a UIViewRepresentable/NSViewRepresentable.

Note

If an accessibility element is not created, the AccessibilityChildBehavior of the existing accessibility element is modified.

## See Also

### Getting behaviors

static let contain: AccessibilityChildBehavior

Any child accessibility elements become children of the new accessibility element.

static let ignore: AccessibilityChildBehavior

Any child accessibility elements become hidden.

