

- Swift
- UnsafePointer
-  pointee 

Instance Property

# pointee

Accesses the instance referenced by this pointer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var pointee: Pointee { get }
```

## Discussion

When reading from the `pointee` property, the instance referenced by this pointer must already be initialized.

