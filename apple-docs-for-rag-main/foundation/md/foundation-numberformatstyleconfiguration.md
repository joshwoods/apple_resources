

- Foundation
-  NumberFormatStyleConfiguration 

Enumeration

# NumberFormatStyleConfiguration

Configuration settings for formatting numbers of different types.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum NumberFormatStyleConfiguration
```

## Overview

This type is effectively a namespace to collect types that configure parts of a formatted number, such as grouping, precision, and separator and sign characters.

## Topics

### Specifying Configuration

struct DecimalSeparatorDisplayStrategy

A structure that an integer format style uses to configure a decimal separator display strategy.

struct Grouping

A structure that an integer format style uses to configure grouping.

struct Precision

A structure that an integer format style uses to configure precision.

typealias RoundingRule

The type used for rounding rule values.

struct SignDisplayStrategy

A structure that an integer format style uses to configure a sign display strategy.

struct Notation

A structure that an integer format style uses to configure notation.

## See Also

### Customizing style behavior

func decimalSeparator(strategy: Decimal.FormatStyle.Configuration.DecimalSeparatorDisplayStrategy) -> Decimal.FormatStyle

Modifies the format style to use the specified decimal separator display strategy.

func grouping(Decimal.FormatStyle.Configuration.Grouping) -> Decimal.FormatStyle

Modifies the format style to use the specified grouping.

func notation(Decimal.FormatStyle.Configuration.Notation) -> Decimal.FormatStyle

Modifies the format style to use the specified notation.

func precision(Decimal.FormatStyle.Configuration.Precision) -> Decimal.FormatStyle

Modifies the format style to use the specified precision.

func rounded(rule: Decimal.FormatStyle.Configuration.RoundingRule, increment: Int?) -> Decimal.FormatStyle

Modifies the format style to use the specified rounding rule and increment.

func scale(Double) -> Decimal.FormatStyle

Modifies the format style to use the specified scale.

func sign(strategy: Decimal.FormatStyle.Configuration.SignDisplayStrategy) -> Decimal.FormatStyle

Modifies the format style to use the specified sign display strategy for displaying or omitting sign symbols.

typealias Configuration

The type the format style uses for configuration settings.

