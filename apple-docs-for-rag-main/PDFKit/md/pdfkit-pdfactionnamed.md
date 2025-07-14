

- PDFKit
-  PDFActionNamed 

Class

# PDFActionNamed

`PDFActionNamed` defines methods used to work with actions in PDF documents, some of which are named in the Adobe PDF Specification.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
class PDFActionNamed
```

## Overview

A `PDFActionNamed` object represents an action with a defined name, such as “Go back” or “Zoom in.”

## Topics

### Accessing the Name of the Action

var name: PDFActionNamedName

Returns the name of the named action.

### Initializing the Action

init(name: PDFActionNamedName)

Initializes the `PDFActionName` object with the specified named action.

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

class PDFActionRemoteGoTo

`PDFActionRemoteGoTo`, a subclass of `PDFAction`, defines methods for getting and setting the destination of a go-to action that targets another document.

class PDFActionResetForm

`PDFActionResetForm`, a subclass of `PDFAction`, defines methods for getting and clearing fields in a PDF form.

class PDFActionURL

`PDFActionURL`, a subclass of `PDFAction`, defines methods for getting and setting the URL associated with a URL action.

enum PDFActionNamedName

