

- Combine
- Future
-  value 

Instance Property

# value

The published value of the future or an error, delivered asynchronously.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
final var value: Output { get async throws }
```

Available when `Failure` conforms to `Error`.

## Discussion

This property subscribes to the `Future` and delivers the value asynchronously when the `Future` publishes it. If the `Future` terminates with an error, the awaiting caller receives the error instead. Use this property when you want to the `async`-`await` syntax with a `Future` whose Failure type is not Never.

## See Also

### Accessing the Value Asynchronously

var value: Output

The published value of the future, delivered asynchronously.

