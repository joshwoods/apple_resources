

- UIKit
- UITextDropRequest
-  isSameView 

Instance Property

# isSameView

A Boolean value indicating whether the drag and the drop are within the same text view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var isSameView: Bool { get }
```

**Required**

## See Also

### Getting information about the text drop request

var dropPosition: UITextPosition

The text position corresponding to the location of a drop session.

**Required**

var suggestedProposal: UITextDropProposal

The text drop proposal offered by the text view.

**Required**

