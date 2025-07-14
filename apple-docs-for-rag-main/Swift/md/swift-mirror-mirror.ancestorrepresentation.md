

- Swift
- Mirror
-  Mirror.AncestorRepresentation 

Enumeration

# Mirror.AncestorRepresentation

The representation to use for ancestor classes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum AncestorRepresentation
```

## Overview

A class that conforms to the `CustomReflectable` protocol can control how its mirror represents ancestor classes by initializing the mirror with an `AncestorRepresentation`. This setting has no effect on mirrors reflecting value type instances.

## Topics

### Enumeration Cases

case customized(() -> Mirror)

Uses the nearest ancestor’s implementation of `customMirror` to create a mirror for that ancestor.

case generated

Generates a default mirror for all ancestor classes.

case suppressed

Suppresses the representation of all ancestor classes.

