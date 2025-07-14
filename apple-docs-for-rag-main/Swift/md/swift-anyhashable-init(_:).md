

- Swift
- AnyHashable
-  init(\_:) 

Initializer

# init(\_:)

Creates a type-erased hashable value that wraps the given instance.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ base: H) where H : Hashable
```

## Parameters 

`base`  

A hashable value to wrap.

