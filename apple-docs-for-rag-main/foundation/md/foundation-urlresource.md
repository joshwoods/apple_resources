

- Foundation
-  URLResource 

Structure

# URLResource

A resource located at a particular file URL within a bundle.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct URLResource
```

## Overview

This type is similar to LocalizedStringResource in its ability to provide access to a resource in a bundle, possibly from another process. Use the URL initializer init(resource:) to resolve the resource.

## Topics

### Creating a URL resource

init(name: String, subdirectory: String?, locale: Locale, bundle: Bundle)

Creates a URL resource from the given bundle, name, and subdirectory, optionally specifying a locale.

### Accessing resource properties

let bundle: Bundle

The bundle containing the resource.

let name: String

The name of the resource in the bundle.

let subdirectory: String?

The subdirectory, if any, of the resource.

var locale: Locale

The bundle containing the resource.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Localization

struct Locale

Information about linguistic, cultural, and technological conventions for use in formatting data for presentation.

class NSOrthography

A description of the linguistic content of natural language text, typically used for spelling and grammar checking.

func NSLocalizedString(String, tableName: String?, bundle: Bundle, value: String, comment: String) -> String

Returns a localized string from a table that Xcode generates for you when exporting localizations.

struct LocalizedStringResource

A reference to a localizable string, accessible from another process.

protocol CustomLocalizedStringResourceConvertible

A type that provides an out-of-process localizable description.

