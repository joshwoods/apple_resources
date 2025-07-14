

- XcodeKit
-  XCSourceEditorExtension 

Protocol

# XCSourceEditorExtension

The protocol you implement to create Xcode source editor extensions.

macOS 10.12+

``` source
protocol XCSourceEditorExtension : NSObjectProtocol
```

## Overview

There are no guarantees about the thread or queue on which any Xcode Source Editor Extension methods are executed, including the designated initializer.

## Topics

### Defining Extension Commands

var commandDefinitions: [[XCSourceEditorCommandDefinitionKey : Any]]

The array of command definitions used by Xcode to associate command names with their implementation in an extension.

### Handling Extension Launches

func extensionDidFinishLaunching()

Tells the extension that it successfully launched and may begin to receive editor commands.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Essentials

Creating a Source Editor Extension

Add and configure a source editor extension in your Xcode project.

Testing Your Source Editor Extension

Launch a special instance of Xcode to test your source editor extension.

