

- Combine
- Future
-  value 

Instance Property

# value

The published value of the future, delivered asynchronously.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
final var value: Output { get async }
```

Available when `Failure` is `Never`.

## Discussion

This property subscribes to the `Future` and delivers the value asynchronously when the `Future` publishes it. Use this property when you want to use the `async`-`await` syntax with a `Future`.

## See Also

### Accessing the Value Asynchronously

var value: Output

The published value of the future or an error, delivered asynchronously.

