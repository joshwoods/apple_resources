

- PDFKit
-  PDFAction 

Class

# PDFAction

An action that is performed when, for example, a PDF annotation is activated or an outline item is clicked.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
class PDFAction
```

## Overview

A `PDFAction` object represents an action associated with a PDF element, such as an annotation or a link, that the viewer application can perform. See the Adobe PDF Specification for more about actions and action types.

`PDFAction` is an abstract superclass of the following concrete classes:

- `PDFActionGoTo`

- `PDFActionNamed`

- `PDFActionRemoteGoTo`

- `PDFActionResetForm`

- `PDFActionURL`

## Topics

### Action Types

class PDFActionGoTo

`PDFActionGoTo`, a subclass of `PDFAction`, defines methods for getting and setting the destination of a go-to action.

class PDFActionNamed

`PDFActionNamed` defines methods used to work with actions in PDF documents, some of which are named in the Adobe PDF Specification.

class PDFActionRemoteGoTo

`PDFActionRemoteGoTo`, a subclass of `PDFAction`, defines methods for getting and setting the destination of a go-to action that targets another document.

class PDFActionResetForm

`PDFActionResetForm`, a subclass of `PDFAction`, defines methods for getting and clearing fields in a PDF form.

class PDFActionURL

`PDFActionURL`, a subclass of `PDFAction`, defines methods for getting and setting the URL associated with a URL action.

enum PDFActionNamedName

### Getting the Action Type

var type: String

Returns the type of the action.

## Relationships

### Inherits From

- NSObject

### Inherited By

- PDFActionGoTo
- PDFActionNamed
- PDFActionRemoteGoTo
- PDFActionResetForm
- PDFActionURL

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Accessing Information About an Annotation

var page: PDFPage?

Returns the page that the annotation is associated with.

var modificationDate: Date?

Returns the modification date of the annotation.

var userName: String?

Returns the name of the user who created the annotation.

var type: String?

Returns the type of the annotation.

var action: PDFAction?

An object that represents an action for a PDF element, such as a link annotation.

class PDFDestination

A `PDFDestination` object describes a point on a PDF page.

