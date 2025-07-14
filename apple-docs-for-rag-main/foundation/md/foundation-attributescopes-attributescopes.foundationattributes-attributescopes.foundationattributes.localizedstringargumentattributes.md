

- Foundation
- AttributeScopes
- AttributeScopes.FoundationAttributes
-  AttributeScopes.FoundationAttributes.LocalizedStringArgumentAttributes 

Structure

# AttributeScopes.FoundationAttributes.LocalizedStringArgumentAttributes

A type for using a localized string argument as an attribute.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct LocalizedStringArgumentAttributes
```

## Overview

You use the this scope’s attributes when creating an attributed string from a LocalizedStringResource. The process creating the attributed string may not have access to the original arguments passed to the interpolation. Instead, the attributed string marks formatted runs with this type, allowing you to retrieve the original values.

## Topics

### Retrieving localization arguments

let localizedNumericArgument: AttributeScopes.FoundationAttributes.LocalizedStringArgumentAttributes.LocalizedNumericArgumentAttribute

The value of a numeric argument used to format the run with this attribute.

enum LocalizedNumericArgumentAttribute

A type for a numeric argument used to format the run with this attribute.

let localizedDateArgument: AttributeScopes.FoundationAttributes.LocalizedStringArgumentAttributes.LocalizedDateArgumentAttribute

The date value used to format the run with this attribute.

enum LocalizedDateArgumentAttribute

A type for a date argument used to format the run with this attribute.

let localizedDateIntervalArgument: AttributeScopes.FoundationAttributes.LocalizedStringArgumentAttributes.LocalizedDateIntervalArgumentAttribute

The date interval value used to format the run with this attribute.

enum LocalizedDateIntervalArgumentAttribute

A type for a date interval argument used to format the run with this attribute.

let localizedURLArgument: AttributeScopes.FoundationAttributes.LocalizedStringArgumentAttributes.LocalizedURLArgumentAttribute

The URL value used to format the run with this attribute.

enum LocalizedURLArgumentAttribute

A type for a URL argument used to format the run with this attribute.

## See Also

### Using string localization attributes

let localizedStringArgumentAttributes: AttributeScopes.FoundationAttributes.LocalizedStringArgumentAttributes

A property for accessing a localized string argument attribute.

