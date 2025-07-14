

- BrowserEngineKit
-  BETextSelectionDirectionNavigation 

Protocol

# BETextSelectionDirectionNavigation

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
protocol BETextSelectionDirectionNavigation
```

## Topics

### Instance Methods

func extend(in: UITextLayoutDirection)

Extends text selection in the specified directions, such as in response to an arrow key press while shift is held.

**Required**

func extend(in: UITextStorageDirection, by: UITextGranularity)

Moves the selection in the specified directions by granularity, in response to different key combinations:

**Required**

func move(in: UITextLayoutDirection)

Moves the cursor in the specified directions, such as in response to an arrow key press.

**Required**

func move(in: UITextStorageDirection, by: UITextGranularity)

Moves the cursor in the specified directions by granularity, in response to different key combinations:

**Required**

## Relationships

### Inherited By

- BETextInput

## See Also

### Text selection

struct BESelectionFlags

enum BESelectionTouchPhase

