

- Combine
- Publishers
- Publishers.Concatenate
-  init(prefix:suffix:) 

Initializer

# init(prefix:suffix:)

Creates a publisher that emits all of one publisher’s elements before those from another publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    prefix: Prefix,
    suffix: Suffix
)
```

## Parameters 

`prefix`  

The publisher to republish, in its entirety, before republishing elements from `suffix`.

`suffix`  

The publisher to republish only after `prefix` finishes.

