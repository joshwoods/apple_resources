

- XcodeKit
-  XCSourceEditorCommand 

Protocol

# XCSourceEditorCommand

The protocol you implement to handle command invocations in a source editor extension.

macOS 10.12+

``` source
protocol XCSourceEditorCommand : NSObjectProtocol
```

## Mentioned in 

Creating a Source Editor Extension

## Overview

A one-to-one mapping between command classes and commands is not required—multiple commands can be handled by a single class, by checking their invocation’s `commandIdentifier` at runtime.

## Topics

### Defining Editor Commands

struct XCSourceEditorCommandDefinitionKey

A key in the dictionary that defines a source editor command.

### Handling Editor Commands

func perform(with: XCSourceEditorCommandInvocation, completionHandler: ((any Error)?) -> Void)

Performs the action associated with the command using the information in an invocation.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Editor Commands

class XCSourceEditorCommandInvocation

An object that identifies the command issued to your extension and provides the contents of the active source editor.

