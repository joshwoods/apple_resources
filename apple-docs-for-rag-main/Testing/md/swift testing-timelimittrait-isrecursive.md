

- Swift Testing
- TimeLimitTrait
-  isRecursive 

Instance Property

# isRecursive

Whether this instance should be applied recursively to child test suites and test functions or should only be applied to the test suite to which it was directly added.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+Swift 6.0+Xcode 16.0+

``` source
var isRecursive: Bool { get }
```

## Discussion

By default, traits are not recursively applied to children.

