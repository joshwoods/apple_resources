

- UIKit
- UISelectionFeedbackGenerator
-  selectionChanged() 

Instance Method

# selectionChanged()

Triggers selection feedback.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
func selectionChanged()
```

## Discussion

This method tells the generator that the user has changed a selection. In response, the generator may play the appropriate haptics. Don’t use this feedback when the user makes or confirms a selection; use it only when the selection changes.

For information on setting up a feedback generator, see the UIFeedbackGenerator class.

## See Also

### Related Documentation

func prepare()

Prepares the generator to trigger feedback.

### Reporting selection changes

func selectionChanged(at: CGPoint)

Triggers selection feedback at the specified location.

