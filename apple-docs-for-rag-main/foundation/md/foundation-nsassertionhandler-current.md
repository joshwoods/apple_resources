

- Foundation
- NSAssertionHandler
-  current 

Type Property

# current

Returns the `NSAssertionHandler` object associated with the current thread.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var current: NSAssertionHandler { get }
```

## Return Value

The `NSAssertionHandler` object associated with the current thread.

## Discussion

If no assertion handler is associated with the current thread, this method creates one and assigns it to the thread.

