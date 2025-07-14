

- Swift
- UnsafeMutablePointer
-  pointer(to:) 

Instance Method

# pointer(to:)

Obtain a mutable pointer to the stored property referred to by a key path.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func pointer(to property: WritableKeyPath) -> UnsafeMutablePointer?
```

## Parameters 

`property`  

A `WritableKeyPath` whose `Root` is `Pointee`.

## Return Value

A mutable pointer to the stored property represented by the key path, or `nil`.

## Discussion

If the key path represents a computed property, this function will return `nil`.

