

- SwiftUI
-  SubmitLabel 

Structure

# SubmitLabel

A semantic label describing the label of submission within a view hierarchy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct SubmitLabel
```

## Overview

A submit label is a description of a submission action provided to a view hierarchy using the onSubmit(of:_:) modifier.

## Topics

### Getting submission labels

static var `continue`: SubmitLabel

Defines a submit label with text of “Continue”.

static var done: SubmitLabel

Defines a submit label with text of “Done”.

static var go: SubmitLabel

Defines a submit label with text of “Go”.

static var join: SubmitLabel

Defines a submit label with text of “Join”.

static var next: SubmitLabel

Defines a submit label with text of “Next”.

static var `return`: SubmitLabel

Defines a submit label with text of “Return”.

static var route: SubmitLabel

Defines a submit label with text of “Route”.

static var search: SubmitLabel

Defines a submit label with text of “Search”.

static var send: SubmitLabel

Defines a submit label with text of “Send”.

## Relationships

### Conforms To

- Sendable

## See Also

### Labeling a submission event

func submitLabel(SubmitLabel) -> some View

Sets the submit label for this view.

