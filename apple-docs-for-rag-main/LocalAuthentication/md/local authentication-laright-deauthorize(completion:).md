

- Local Authentication
- LARight
-  deauthorize(completion:) 

Instance Method

# deauthorize(completion:)

Invalidates a previously authorized right.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func deauthorize(completion handler: @escaping () -> Void)
```

``` source
func deauthorize() async
```

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func deauthorize() async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

