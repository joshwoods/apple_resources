

- HealthKit
-  HKCDADocument 

Class

# HKCDADocument

An object representing a Clinical Document Architecture (CDA) document in HealthKit.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+

``` source
class HKCDADocument
```

## Overview

CDA documents use XML to encode clinical documents so that they can be easily exchanged. For more information on the CDA document format, see the Clinical Document Architecture, R2 standard.

Do not instantiate `HKCDADocument` objects directly. Instead, create a new HKCDADocumentSample object by calling the init(data:start:end:metadata:) method, and passing the CDA’s XML data. HealthKit creates a `HKCDADocument` object for the XML, and assigns it to the sample’s document property.

`HKCDADocument` objects are immutable. When you create a new document sample, HealthKit parses the title, patient name, author name, and custodian name from the XML to populates the document object’s properties. These properties cannot be changed.

Like many HealthKit classes, the HKCDADocument class should not be subclassed.

## Topics

### Accessing the Document’s Data

var authorName: String

The document’s author.

var custodianName: String

The name of the organization responsible for the document.

var documentData: Data?

The CDA document stored as XML data.

var patientName: String

The patient’s name.

var title: String

The document’s title.

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
- Sendable

## See Also

### Accessing the Document

var document: HKCDADocument?

The CDA document.

