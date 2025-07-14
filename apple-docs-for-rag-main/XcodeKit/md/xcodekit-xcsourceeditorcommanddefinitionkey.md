

- XcodeKit
-  XCSourceEditorCommandDefinitionKey 

Structure

# XCSourceEditorCommandDefinitionKey

A key in the dictionary that defines a source editor command.

macOS 10.12+

``` source
struct XCSourceEditorCommandDefinitionKey
```

## Mentioned in 

Creating a Source Editor Extension

## Overview

Source editor commands are defined via an array of dictionaries under the `XCSourceEditorCommandDefinitions` key of a Xcode Source Editor Extension’s `NSExtensionAttributes` within its `Info.plist` file. Commands can also be specified via the commandDefinitions property in an extension’s conformance to the XCSourceEditorExtension protocol.

## Topics

### Populating a Command Definition Dictionary

static let classNameKey: XCSourceEditorCommandDefinitionKey

The class of the source editor command, in its attributes.

static let identifierKey: XCSourceEditorCommandDefinitionKey

The identifier of the source editor command in its attributes.

static let nameKey: XCSourceEditorCommandDefinitionKey

The name of the source editor command in its attributes.

### Creating a Key Using a Raw String

init(rawValue: String)

Creates the key for a source-editor command by using the string value you specify.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

