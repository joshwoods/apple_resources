

- Shared With You
-  SWHighlight 

Class

# SWHighlight

An object that represents a universal link to share by any number of contacts in one or more conversations.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class SWHighlight
```

## Mentioned in 

Adding shared content collaboration to your app

Making your app content shareable

## Overview

The system doesn’t expose the identities of the contacts to the app. It tracks shared universal links for the current user and determines which links to elevate for consumption in an app. When the system deems a link to be useful, it surfaces that link to the hosting app in the form of an `SWHighlight` object.

## Topics

### Viewing highlight attributes

var identifier: any NSCopying &amp; NSSecureCoding

The unique identifier for the highlight.

var url: URL

The surfaced content URL for the highlight.

## Relationships

### Inherits From

- NSObject

### Inherited By

- SWCollaborationHighlight

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Highlights

class SWHighlightCenter

An object that contains a priority-ordered list of universal links to share with the current user.

