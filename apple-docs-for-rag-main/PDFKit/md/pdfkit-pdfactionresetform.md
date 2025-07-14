

- PDFKit
-  PDFActionResetForm 

Class

# PDFActionResetForm

`PDFActionResetForm`, a subclass of `PDFAction`, defines methods for getting and clearing fields in a PDF form.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
class PDFActionResetForm
```

## Overview

A `PDFActionResetForm` object represents an action associated with a PDF form.

## Topics

### Initializing a Reset Form Action

init()

Initializes a reset form action.

### Accessing and Changing Fields

var fields: [String]?

Returns an array of fields associated with the reset action.

### Determining Whether Fields are Cleared When the Action is Performed

var fieldsIncludedAreCleared: Bool

Sets whether the fields associated with the reset action are cleared when the action is performed.

## Relationships

### Inherits From

- PDFAction

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Action Types

class PDFActionGoTo

`PDFActionGoTo`, a subclass of `PDFAction`, defines methods for getting and setting the destination of a go-to action.

class PDFActionNamed

`PDFActionNamed` defines methods used to work with actions in PDF documents, some of which are named in the Adobe PDF Specification.

class PDFActionRemoteGoTo

`PDFActionRemoteGoTo`, a subclass of `PDFAction`, defines methods for getting and setting the destination of a go-to action that targets another document.

class PDFActionURL

`PDFActionURL`, a subclass of `PDFAction`, defines methods for getting and setting the URL associated with a URL action.

enum PDFActionNamedName

