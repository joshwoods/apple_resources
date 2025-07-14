

- SwiftUI
- Text
-  accessibilityLabel(\_:) 

Instance Method

# accessibilityLabel(\_:)

Adds a label to the view that describes its contents.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func accessibilityLabel(_ label: Text) -> Text
```

Show all declarations

## Parameters 

`label`  

The text view to add the label to.

## Discussion

Use this method to provide an alternative accessibility label to the text that is displayed. For example, you can give an alternate label to a navigation title:

```
var body: some View {
    NavigationView {
        ContentView()
            .navigationTitle(Text("􀈤").accessibilityLabel("Inbox"))
    }
}
```

You can’t style the label that you add

## See Also

### Providing accessibility information

func accessibilityHeading(AccessibilityHeadingLevel) -> Text

Sets the accessibility level of this heading.

func accessibilityTextContentType(AccessibilityTextContentType) -> Text

Sets an accessibility text content type.

