

- AppKit
- NSWritingToolsCoordinator
-  updateForReflowedTextInContextWithIdentifier(\_:) 

Instance Method

# updateForReflowedTextInContextWithIdentifier(\_:)

Informs the coordinator that a change occurred to the view or its text that requires a layout update.

macOS 15.2+

``` source
@MainActor
func updateForReflowedTextInContextWithIdentifier(_ contextID: UUID)
```

## Parameters 

`contextID`  

The unique identifier of the context object affected by the change. Pass the identifier for the context object that comes after the changes.

## Mentioned in 

Adding Writing Tools support to a custom AppKit view

## Discussion

Use this method to inform Writing Tools when the geometry of your view changes, or when the text that precedes one of your context objects changes. Changes to the view’s geometry or text can affect the flow of any remaining text, and require a layout update. Writing Tools uses this method to refresh any layout-dependent information it’s currently tracking. For example, it uses it to refresh the location of proofreading marks it’s displaying in your view.

If a text change affects the text inside a context object, call the updateRange(_:with:reason:forContextWithIdentifier:) method to report that change instead.

## See Also

### Reporting changes to Writing Tools

func updateRange(NSRange, with: NSAttributedString, reason: NSWritingToolsCoordinator.TextUpdateReason, forContextWithIdentifier: UUID)

Informs the coordinator about changes your app made to the text in the specified context object.

enum TextUpdateReason

Constants that specify the reason you updated your view’s content outside of the Writing Tools workflow.

