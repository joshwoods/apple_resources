

- Messages
-  MSMessageLayout 

Class

# MSMessageLayout

An abstract base class that defines the appearance of MSMessage objects in the conversation transcript.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
class MSMessageLayout
```

## Overview

You do not subclass `MSMessageLayout` or create instances of it directly. Instead, instantiate the provided concrete subclass, the MSMessageTemplateLayout class.

## Relationships

### Inherits From

- NSObject

### Inherited By

- MSMessageLiveLayout
- MSMessageTemplateLayout

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Interactive messages

class MSMessage

A custom message object.

class MSSession

A session object used to create and update messages.

class MSMessageTemplateLayout

A template-based layout for custom messages.

class MSMessageLiveLayout

A layout that provides a custom, interactive view inside the transcript.

