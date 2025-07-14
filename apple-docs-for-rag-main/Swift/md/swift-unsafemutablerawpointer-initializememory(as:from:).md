

- Swift
- UnsafeMutableRawPointer
-  initializeMemory(as:from:) 

Instance Method

# initializeMemory(as:from:)

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
func initializeMemory(
    as type: C.Element.Type,
    from source: C
) -> UnsafeMutablePointer where C : Collection
```

