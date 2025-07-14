

- Core Text
-  CTUnderlineStyle 

Structure

# CTUnderlineStyle

Underline style specifiers.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CTUnderlineStyle
```

## Overview

You can apply these underline style specifiers to the value that you set with the kCTUnderlineStyleAttributeName attribute. These specifiers control the underline style Core Text uses when rendering the text to which the attribute applies.

## Topics

### Constants

static var single: CTUnderlineStyle

A specifier that indicates to draw an underline consisting of a single line.

static var thick: CTUnderlineStyle

A specifier that indicates to draw an underline consisting of a thick line.

static var double: CTUnderlineStyle

A specifier that indicates to draw an underline consisting of a double line.

### Initializers

init(rawValue: Int32)

Creates an underline style structure with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Constants

String Attribute Name Constants

These constants represent string attribute names.

struct CTUnderlineStyleModifiers

Underline style modifiers.

