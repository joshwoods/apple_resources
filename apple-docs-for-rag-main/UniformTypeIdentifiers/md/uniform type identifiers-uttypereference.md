

- Uniform Type Identifiers
-  UTTypeReference 

Class

# UTTypeReference

An object that represents a type of data to load, send, or receive.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class UTTypeReference
```

## Overview

The UTTypeReference object may represent files on disk, abstract data types with no on-disk representation, or entirely unrelated hierarchical classification systems, such as hardware. Each instance has a unique identifier, and helpful properties, preferredFilenameExtension and preferredMIMEType.

Note

The system includes static declarations for many common types, which you can look up by identifier, filename extension, or MIME type.

The UTTypeReference object may provide additional information related to the type. For example, it may include a localized user-facing description, a reference URL to technical documentation about the type, or its version number. You can look up types by their conformance to get either a type or a list of types that are relevant to your use case.

To define your own types in your app’s `Info.plist`, see Defining file and data types for your app.

## Topics

### Looking up a type

class func types(tag: String, tagClass: String, conformingTo: UTType?) -> [UTType]

Returns an array of types from the provided tag and tag class.

### Creating a type

convenience init?(String)

Creates a type based on an identifier.

convenience init?(mimeType: String)

Creates a type based on a MIME type.

convenience init?(mimeType: String, conformingTo: UTType)

Creates a type based on a MIME type and a supertype that it conforms to.

convenience init?(filenameExtension: String)

Creates a type that represents the specified filename extension.

convenience init?(filenameExtension: String, conformingTo: UTType)

Creates a type that represents the specified filename extension and conforms to an existing type.

convenience init?(tag: String, tagClass: String, conformingToType: UTType?)

Creates a type that represents the specified tag and tag class and which conforms to an existing type.

init(exportedAs: String)

Creates a type your app owns based on an identifier.

init(exportedAs: String, conformingTo: UTType)

Creates a type your app owns based on an identifier and a supertype that it conforms to.

init(importedAs: String)

Creates a type your app uses, but doesn’t own, based on an identifier.

init(importedAs: String, conformingTo: UTType)

Creates a type your app uses, but doesn’t own, based on an identifier and a supertype that it conforms to.

### Identifying a type

var identifier: String

The string that represents the type.

### Obtaining tags

var preferredFilenameExtension: String?

The preferred filename extension for the type.

var preferredMIMEType: String?

The preferred MIME type for the type.

var tags: [UTTagClass : [String]]

The tag specification dictionary of the type.

### Obtaining additional type information

var isDeclared: Bool

A Boolean value that indicates whether the system declares the type.

var isDynamic: Bool

A Boolean value that indicates whether the system generates the type.

var isPublic: Bool

A Boolean value that indicates whether the type is in the public domain.

var referenceURL: URL?

The reference URL for the type.

var version: Int?

The type’s version, if available.

### Checking a type’s relationship to another type

var supertypes: Set&lt;UTType>

The set of types the type directly or indirectly conforms to.

func conforms(to: UTType) -> Bool

Returns a Boolean value that indicates whether a type conforms to the type.

func isSubtype(of: UTType) -> Bool

Returns a Boolean value that indicates whether a type is higher in a hierarchy than the type.

func isSupertype(of: UTType) -> Bool

Returns a Boolean value that indicates whether a type is lower in a hierarchy than the type.

### Describing a type

var localizedDescription: String?

A localized description of the type.

### Type Properties

static var shazamCustomCatalog: UTType

A type that represents a custom catalog.

static var shazamSignature: UTType

A type that represents a signature.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Uniform type identifiers

struct UTType

A structure that represents a type of data to load, send, or receive.

struct UTTagClass

A type that represents tag classes.

