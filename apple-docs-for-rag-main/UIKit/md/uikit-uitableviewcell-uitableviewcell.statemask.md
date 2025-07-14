

- UIKit
- UITableViewCell
-  UITableViewCell.StateMask 

Structure

# UITableViewCell.StateMask

Constants used to determine the new state of a cell as it transitions between states.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct StateMask
```

## Overview

The methods that use these constants are didTransition(to:) and willTransition(to:).

## Topics

### Constants

static var showingEditControl: UITableViewCell.StateMask

The state of a table view cell when the table view is in editing mode.

static var showingDeleteConfirmation: UITableViewCell.StateMask

The state of a table view cell that shows a button requesting confirmation of a delete gesture.

### Initializers

init(rawValue: UInt)

Creates a state mask with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Adjusting to state transitions

func willTransition(to: UITableViewCell.StateMask)

Notifies the cell that it’s about to transition to a new cell state.

func didTransition(to: UITableViewCell.StateMask)

Notifies the cell that it transitioned to a new cell state.

