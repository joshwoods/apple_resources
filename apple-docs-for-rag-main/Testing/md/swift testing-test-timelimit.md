

- Swift Testing
- Test
-  timeLimit 

Instance Property

# timeLimit

The maximum amount of time the cases of this test may run for.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+Swift 6.0+Xcode 16.0+

``` source
var timeLimit: Duration? { get }
```

## Discussion

Time limits are associated with tests using this trait:

- timeLimit(_:)

If a test has more than one time limit associated with it, the value of this property is the shortest one. If a test has no time limits associated with it, the value of this property is `nil`.

