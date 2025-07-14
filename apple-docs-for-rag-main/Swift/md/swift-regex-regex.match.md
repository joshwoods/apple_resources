

- Swift
- Regex
-  Regex.Match 

Structure

# Regex.Match

The result of matching a regular expression against a string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@dynamicMemberLookup
struct Match
```

## Overview

A `Match` forwards API to the `Output` generic parameter, providing direct access to captures.

## Topics

### Initializers

init&lt;OtherOutput>(Regex&lt;OtherOutput>.Match)

Creates a regular expression match with a dynamic capture list from the given match.

### Instance Properties

var output: Output

The output produced from the match operation.

let range: Range&lt;String.Index>

The range of the overall match.

### Subscripts

subscript(String) -> AnyRegexOutput.Element?

Accesses the capture with the specified name, if a capture with that name exists.

subscript&lt;Capture>(Reference&lt;Capture>) -> Capture

Accesses this match’s capture by the given reference.

subscript&lt;T>(dynamicMember _: KeyPath&lt;Output, T>) -> T

Accesses a capture by its name or number.

