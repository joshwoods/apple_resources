

- UIKit
- UITextDropProposal
-  UITextDropProposal.Performer 

Enumeration

# UITextDropProposal.Performer

The performers that are responsible for handling the drop operation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum Performer
```

## Overview

A performer is responsible for:

- Proving a preview for the drop activity.

- Loading data from the item providers.

- Inserting the data into the text view.

## Topics

### Performers

case view

A performer type that indicates that the text view is responsible for doing the drop operation.

case delegate

A performer type that indicates the delegate object is responsible for doing the drop operation.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Drop management

protocol UITextDropRequest

The interface for specifying the attributes of a drop request for a text view.

class UITextDropProposal

A proposed configuration for the behavior of a text drop interaction.

enum Action

The text drop action styles for text views.

enum ProgressMode

The text drop progress styles for user-visible progress indication.

