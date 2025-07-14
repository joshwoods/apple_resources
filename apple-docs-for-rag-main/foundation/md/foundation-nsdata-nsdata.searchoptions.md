

- Foundation
- NSData
-  NSData.SearchOptions 

Structure

# NSData.SearchOptions

Options for method used to search data objects.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct SearchOptions
```

## Overview

These options are used with the range(of:options:in:) method.

## Topics

### Initializers

init(rawValue: UInt)

### Constants

static var backwards: NSData.SearchOptions

Search from the end of the data object.

static var anchored: NSData.SearchOptions

Search is limited to start (or end, if searching backwards) of the data object.

static var backwards: NSData.SearchOptions

Search from the end of the data object.

static var anchored: NSData.SearchOptions

Search is limited to start (or end, if searching backwards) of the data object.

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

### Finding Data

func subdata(with: NSRange) -> Data

Returns a new data object containing the data object’s bytes that fall within the limits specified by a given range.

func range(of: Data, options: NSData.SearchOptions, in: NSRange) -> NSRange

Finds and returns the range of the first occurrence of the given data, within the given range, subject to given options.

