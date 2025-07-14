

- Core Foundation
-  CFURLBookmarkCreationOptions 

Structure

# CFURLBookmarkCreationOptions

Type for bookmark data creation options.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct CFURLBookmarkCreationOptions
```

## Overview

See Bookmark Data Creation Options for possible values.

## Topics

### Initializers

init(rawValue: CFOptionFlags)

### Type Properties

static var minimalBookmarkMask: CFURLBookmarkCreationOptions

Specifies that an alias created with the bookmark data be created with minimal information, which may make it smaller but still able to resolve in certain ways.

static var preferFileIDResolutionMask: CFURLBookmarkCreationOptions

Specifies that an alias created with the bookmark data prefers resolving with its embedded file ID.

Deprecated

static var securityScopeAllowOnlyReadAccess: CFURLBookmarkCreationOptions

When combined with the withSecurityScope option, specifies that you want to create a security-scoped bookmark that, when resolved, provides a security-scoped URL allowing read-only access to a file-system resource; for use in an app that adopts App Sandbox.

static var suitableForBookmarkFile: CFURLBookmarkCreationOptions

Specifies that the bookmark data include properties required to create Finder alias files.

static var withSecurityScope: CFURLBookmarkCreationOptions

Specifies that you want to create a security-scoped bookmark that, when resolved, provides a security-scoped URL allowing read/write access to a file-system resource; for use in an app that adopts App Sandbox.

static var withoutImplicitSecurityScope: CFURLBookmarkCreationOptions

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

typealias CFURLBookmarkFileCreationOptions

Type for bookmark file creation options.

struct CFURLBookmarkResolutionOptions

Type for bookmark data resolution options.

