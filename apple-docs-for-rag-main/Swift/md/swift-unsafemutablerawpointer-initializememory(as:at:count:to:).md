

- Swift
- UnsafeMutableRawPointer
-  initializeMemory(as:at:count:to:) 

Instance Method

# initializeMemory(as:at:count:to:)

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
func initializeMemory(
    as type: T.Type,
    at offset: Int = 0,
    count: Int = 1,
    to repeatedValue: T
) -> UnsafeMutablePointer
```

