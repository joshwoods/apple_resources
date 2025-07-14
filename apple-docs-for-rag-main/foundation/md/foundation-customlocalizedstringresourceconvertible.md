

- Foundation
-  CustomLocalizedStringResourceConvertible 

Protocol

# CustomLocalizedStringResourceConvertible

A type that provides an out-of-process localizable description.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol CustomLocalizedStringResourceConvertible
```

## Overview

Similar to CustomStringConvertible, types that conform to CustomLocalizedStringResourceConvertible provide their own representation when converting to a string instance. Whereas CustomStringConvertible provides a description string, this type offers a LocalizedStringResource. This allows out-of-process callers to create a localized description from the resource, possibly in a different locale than the current process uses.

## Topics

### Describing a resource

var localizedStringResource: LocalizedStringResource

A resource that helps provide a description of this instance.

**Required**

## Relationships

### Conforming Types

- LocalizedStringResource

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

struct URLResource

A resource located at a particular file URL within a bundle.

