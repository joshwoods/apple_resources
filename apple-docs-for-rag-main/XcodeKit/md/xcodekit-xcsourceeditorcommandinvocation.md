

- XcodeKit
-  XCSourceEditorCommandInvocation 

Class

# XCSourceEditorCommandInvocation

An object that identifies the command issued to your extension and provides the contents of the active source editor.

macOS 10.12+

``` source
class XCSourceEditorCommandInvocation
```

## Topics

### Responding to Commands

var buffer: XCSourceTextBuffer

The buffer of source text upon which the command can operate.

var commandIdentifier: String

The identifier of the command that the user invoked.

### Responding to Cancelled Commands

var cancellationHandler: () -> Void

A handler to be invoked by Xcode to indicate that the invocation has been canceled by the user.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Editor Commands

protocol XCSourceEditorCommand

The protocol you implement to handle command invocations in a source editor extension.

