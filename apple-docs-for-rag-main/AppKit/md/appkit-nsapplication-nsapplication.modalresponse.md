

- AppKit
- NSApplication
-  NSApplication.ModalResponse 

Structure

# NSApplication.ModalResponse

A set of button return values for modal dialogs.

macOS

``` source
struct ModalResponse
```

## Discussion

The response value that a button returns can depend on which method is used to present the dialog. See alertWithMessageText:defaultButton:alternateButton:otherButton:informativeTextWithFormat:, runModal(), and addButton(withTitle:) for examples.

## Topics

### Responses

static let OK: NSApplication.ModalResponse

The presentation or dismissal of the sheet has finished.

static let cancel: NSApplication.ModalResponse

The presentation or dismissal of the sheet has been canceled.

static let `continue`: NSApplication.ModalResponse

Modal session is continuing (returned by runModalSession(_:) only).

static let stop: NSApplication.ModalResponse

Modal session was broken with stopModal().

static let abort: NSApplication.ModalResponse

Modal session was broken with abortModal().

static let alertFirstButtonReturn: NSApplication.ModalResponse

The user clicked the first (rightmost) button on the dialog or sheet.

static let alertSecondButtonReturn: NSApplication.ModalResponse

The user clicked the second button from the right edge of the dialog or sheet.

static let alertThirdButtonReturn: NSApplication.ModalResponse

The user clicked the third button from the right edge of the dialog or sheet.

### Deprecated Responses

var NSRunStoppedResponse: Int

Modal session was broken with stopModal().

Deprecated

var NSRunAbortedResponse: Int

Modal session was broken with abortModal().

Deprecated

var NSRunContinuesResponse: Int

Modal session is continuing (returned by runModalSession(_:) only).

Deprecated

### Initializers

init(Int)

init(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum Style

The set of alert styles to style alerts in your app.

