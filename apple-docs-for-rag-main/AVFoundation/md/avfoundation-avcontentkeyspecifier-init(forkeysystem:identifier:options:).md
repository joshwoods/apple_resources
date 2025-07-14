

- AVFoundation
- AVContentKeySpecifier
-  init(forKeySystem:identifier:options:) 

Initializer

# init(forKeySystem:identifier:options:)

Creates a content key specifier.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+watchOS 7.4+

``` source
init(
    forKeySystem keySystem: AVContentKeySystem,
    identifier contentKeyIdentifier: Any,
    options: [String : Any] = [:]
)
```

## Parameters 

`keySystem`  

The key system to use to generate content keys.

`contentKeyIdentifier`  

The container and protocol-specific key identifier.

`options`  

Additional information necessary to obtain the key. Pass `nil` to indicate no additional options.

