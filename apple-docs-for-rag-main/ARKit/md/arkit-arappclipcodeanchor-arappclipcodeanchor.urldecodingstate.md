

- ARKit
- ARAppClipCodeAnchor
-  ARAppClipCodeAnchor.URLDecodingState 

Enumeration

# ARAppClipCodeAnchor.URLDecodingState

The states in the process of decoding an App Clip code URL.

iOS 14.3+iPadOS 14.3+Mac Catalyst 14.3+

``` source
enum URLDecodingState
```

## Overview

The possible states of decoding the url of an App Clip Code.

## Topics

### States

case decoded

A state that indicates the completed decoding of an App Clip Code URL.

case decoding

A state that indicates the continuing process of decoding an App Clip Code’s URL.

case failed

A state that indicates the failure to decode an App Clip Code’s URL.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Decoding the URL

var url: URL?

The URL encoded in an App Clip Code.

var urlDecodingState: ARAppClipCodeAnchor.URLDecodingState

A state that indicates the process of decoding an App Clip Code URL.

