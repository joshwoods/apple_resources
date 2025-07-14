

- SwiftUI
-  RenameAction 

Structure

# RenameAction

An action that activates a standard rename interaction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct RenameAction
```

## Overview

Use the renameAction(_:) modifier to configure the rename action in the environment.

## Topics

### Calling the action

func callAsFunction()

Triggers the standard rename action provided through the environment.

## See Also

### Renaming a document

struct RenameButton

A button that triggers a standard rename action.

func renameAction(_:)

Sets a closure to run for the rename action.

var rename: RenameAction?

An action that activates the standard rename interaction.

