

- Swift
- ManagedBuffer
-  create(minimumCapacity:makingHeaderWith:) 

Type Method

# create(minimumCapacity:makingHeaderWith:)

Create a new instance of the most-derived class, calling `factory` on the partially-constructed object to generate an initial `Header`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
final class func create(
    minimumCapacity: Int,
    makingHeaderWith factory: (ManagedBuffer) throws -> Header
) rethrows -> ManagedBuffer
```

