

- Core Foundation
-  CFURLBookmarkResolutionOptions 

Structure

# CFURLBookmarkResolutionOptions

Type for bookmark data resolution options.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct CFURLBookmarkResolutionOptions
```

## Overview

See Bookmark Data Resolution Options for possible values.

## Topics

### Initializers

init(rawValue: CFOptionFlags)

### Type Properties

static var cfBookmarkResolutionWithoutMountingMask: CFURLBookmarkResolutionOptions

Specifies that no volume should be mounted during resolution of the bookmark data.

static var cfBookmarkResolutionWithoutUIMask: CFURLBookmarkResolutionOptions

Specifies that no UI feedback accompany resolution of the bookmark data.

static var cfurlBookmarkResolutionWithSecurityScope: CFURLBookmarkResolutionOptions

Specifies that the security scope, applied to the bookmark when it was created, should be used during resolution of the bookmark data.

static var cfurlBookmarkResolutionWithoutImplicitStartAccessing: CFURLBookmarkResolutionOptions

static var cfurlBookmarkResolutionWithoutMountingMask: CFURLBookmarkResolutionOptions

static var cfurlBookmarkResolutionWithoutUIMask: CFURLBookmarkResolutionOptions

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

### Bookmark Data Types

struct CFURLBookmarkCreationOptions

Type for bookmark data creation options.

typealias CFURLBookmarkFileCreationOptions

Type for bookmark file creation options.

