

- UIKit
- UITextView
-  findInteraction 

Instance Property

# findInteraction

The text view’s built-in find interaction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var findInteraction: UIFindInteraction? { get }
```

## Discussion

Set isFindInteractionEnabled to `true` to enable the text view’s built-in find interaction. This method returns `nil` when the interaction isn’t enabled.

Call presentFindNavigator(showingReplace:) on the UIFindInteraction object returned by this method to invoke the find interaction and display the find panel.

## See Also

### Supporting Find and Replace

var isFindInteractionEnabled: Bool

A Boolean value that enables a text view’s built-in find interaction.

