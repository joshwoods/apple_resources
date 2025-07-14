

- Core Text
-  CTUnderlineStyleModifiers 

Structure

# CTUnderlineStyleModifiers

Underline style modifiers.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CTUnderlineStyleModifiers
```

## Overview

You can apply these underline style modifiers to the underline style (CTUnderlineStyle) that you set with the kCTUnderlineStyleAttributeName attribute. These modifiers control the pattern of the underline.

## Topics

### Constants

static var patternSolid: CTUnderlineStyleModifiers

A modifier that indicates to draw a solid underline.

static var patternDot: CTUnderlineStyleModifiers

A modifier that indicates to draw an underline using a pattern of dots.

static var patternDash: CTUnderlineStyleModifiers

A modifier that indicates to draw an underline using a pattern of dashes.

static var patternDashDot: CTUnderlineStyleModifiers

A modifier that indicates to draw an underline using a pattern of alternating dashes and dots.

static var patternDashDotDot: CTUnderlineStyleModifiers

A modifier that indicates to draw an underline using a pattern of a dash followed by two dots.

### Initializers

init(rawValue: Int32)

Creates an underline style modifiers structure with the specified raw value.

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

struct CTUnderlineStyle

Underline style specifiers.

