

- SwiftUI
- Text input and output
- TextField
-  Deprecated initializers 

API Collection

# Deprecated initializers

Review deprecated text field initializers.

## Overview

Use view modifiers to specify change and commit behaviors for a text field when replacing these initializers. Use the onSubmit(of:_:) view modifier to get the behavior provided by the `onCommit` parameter. Use focused(_:equals:) and FocusState to get the behavior provided by the `onEditingChanged` parameter.

## Topics

### Creating a text field with a string

init(_:text:onEditingChanged:onCommit:)

Creates a text field with a text label generated from a localized title string.

Deprecated

init(_:text:onCommit:)

Creates a text field with a text label generated from a localized title string.

Deprecated

init(_:text:onEditingChanged:)

Creates a text field with a text label generated from a localized title string.

Deprecated

### Creating a text field with a value

init(_:value:formatter:onEditingChanged:onCommit:)

Creates an instance which binds over an arbitrary type, `T`.

Deprecated

init(_:value:formatter:onCommit:)

Create an instance which binds over an arbitrary type, `V`.

Deprecated

init(_:value:formatter:onEditingChanged:)

Create an instance which binds over an arbitrary type, `V`.

Deprecated

