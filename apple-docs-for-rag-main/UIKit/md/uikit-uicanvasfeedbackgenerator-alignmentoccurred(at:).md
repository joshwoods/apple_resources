

- UIKit
- UICanvasFeedbackGenerator
-  alignmentOccurred(at:) 

Instance Method

# alignmentOccurred(at:)

Triggers feedback to indicate when an alignment occurs, such as snapping an object to a guide or ruler.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+

``` source
@MainActor
func alignmentOccurred(at location: CGPoint)
```

## See Also

### Reporting canvas events

func pathCompleted(at: CGPoint)

Triggers feedback to indicate path completion or shape recognition.

