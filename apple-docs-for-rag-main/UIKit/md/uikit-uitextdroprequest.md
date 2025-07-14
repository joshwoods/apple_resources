

- UIKit
-  UITextDropRequest 

Protocol

# UITextDropRequest

The interface for specifying the attributes of a drop request for a text view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UITextDropRequest : NSObjectProtocol
```

## Topics

### Getting information about the text drop request

var dropPosition: UITextPosition

The text position corresponding to the location of a drop session.

**Required**

var isSameView: Bool

A Boolean value indicating whether the drag and the drop are within the same text view.

**Required**

var suggestedProposal: UITextDropProposal

The text drop proposal offered by the text view.

**Required**

### Getting the drop session

var dropSession: any UIDropSession

The drop session for the text view.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Drop management

class UITextDropProposal

A proposed configuration for the behavior of a text drop interaction.

enum Action

The text drop action styles for text views.

enum Performer

The performers that are responsible for handling the drop operation.

enum ProgressMode

The text drop progress styles for user-visible progress indication.

