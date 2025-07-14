

- PassKit (Apple Pay and Wallet)
-  PKIdentityDocumentDescriptor 

Protocol

# PKIdentityDocumentDescriptor

A type that describes the structure and behavior of an identity document.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
protocol PKIdentityDocumentDescriptor : NSObjectProtocol
```

## Overview

A descriptor object describes the type of document that your app can request or check whether a document is available to request. For example, you use a PKIdentityDriversLicenseDescriptor to request information from a user’s driver’s license (or equivalent document).

Note

Different document types behave differently, requiring different properties or response formats. Don’t define your own implementation of this protocol or subclass an existing implementation.

## Topics

### Inspecting elements

var elements: [PKIdentityElement]

A list of identity elements to request.

**Required**

class PKIdentityElement

An object that represents the elements an app requests from identity documents.

### Adding an identity element

func addElements([PKIdentityElement], intentToStore: PKIdentityIntentToStore)

Adds a list of identity element and defines the way an app, or it’s server, stores the elements.

**Required**

class PKIdentityIntentToStore

An object that represents your intention to store an identity element or values derived from an identity element.

### Getting an elements intent

func intentToStore(element: PKIdentityElement) -> PKIdentityIntentToStore?

Gets the intent to store for an identity element you specify.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- PKIdentityDriversLicenseDescriptor
- PKIdentityNationalIDCardDescriptor

## See Also

### Describing a document

class PKIdentityDriversLicenseDescriptor

An object for requesting information from a user’s driver’s license or equivalent document.

class PKIdentityIntentToStore

An object that represents your intention to store an identity element or values derived from an identity element.

