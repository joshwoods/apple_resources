

- Foundation
- AttributeScopes
- AttributeScopes.FoundationAttributes
-  AttributeScopes.FoundationAttributes.ReplacementIndexAttribute 

Enumeration

# AttributeScopes.FoundationAttributes.ReplacementIndexAttribute

A type for using a replacement index as an attribute.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
enum ReplacementIndexAttribute
```

## Overview

When you use the applyReplacementIndexAttribute formatting option, the resulting formatted string uses this attribute to mark the location of replacement strings. This allows you to relate ranges to replacements even if localizers change the word order in format strings.

## Relationships

### Conforms To

- AttributedStringKey
- BitwiseCopyable
- Copyable
- DecodableAttributedStringKey
- EncodableAttributedStringKey

## See Also

### Using string formatting attributes

let replacementIndex: AttributeScopes.FoundationAttributes.ReplacementIndexAttribute

A property for accessing a replacement index attribute.

