

- SwiftUI
- AccessibilityChildBehavior
-  ignore 

Type Property

# ignore

Any child accessibility elements become hidden.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let ignore: AccessibilityChildBehavior
```

## Discussion

Use this behavior when you want a view represented by a single accessibility element. The new accessibility element has no initial properties. So you will need to use other accessibility modifiers, such as accessibilityLabel(_:), to begin making it accessible.

```
var body: some View {
    VStack {
        Button("Previous Page", action: goBack)
        Text("\(pageNumber)")
        Button("Next Page", action: goForward)
    }
    .accessibilityElement(children: .ignore)
    .accessibilityValue("Page \(pageNumber) of \(pages.count)")
    .accessibilityAdjustableAction { action in
        if action == .increment {
            goForward()
        } else {
            goBack()
        }
    }
}
```

Before using the ignorebehavior, consider using the combine behavior.

Note

A new accessibility element is always created.

## See Also

### Getting behaviors

static let combine: AccessibilityChildBehavior

Any child accessibility element’s properties are merged into the new accessibility element.

static let contain: AccessibilityChildBehavior

Any child accessibility elements become children of the new accessibility element.

