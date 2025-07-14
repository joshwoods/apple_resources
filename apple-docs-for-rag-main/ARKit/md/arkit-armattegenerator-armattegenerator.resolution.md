

- ARKit
- ARMatteGenerator
-  ARMatteGenerator.Resolution 

Enumeration

# ARMatteGenerator.Resolution

A resolution for a matte texture.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
enum Resolution
```

## Overview

You generate a matte texture every frame, specifying whether its resolution is the full size or half of the camera image.

## Topics

### Choosing a Resolution Option

case full

An option that specifies the full camera image resolution.

case half

An option that specifies half of the camera image resolution.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

