

- Combine
- Publishers
- Publishers.DropWhile
-  values 

Instance Property

# values

The elements produced by the publisher, as an asynchronous sequence.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
var values: AsyncPublisher { get }
```

Available when `Failure` is `Never`.

## Discussion

This property provides an AsyncPublisher, which allows you to use the Swift `async`-`await` syntax to receive the publisher’s elements. Because AsyncPublisher conforms to AsyncSequence, you iterate over its elements with a `for`-`await`-`in` loop, rather than attaching a subscriber.

The following example shows how to use the `values` property to receive elements asynchronously. The example adapts a code snippet from the filter(_:) operator’s documentation, which filters a sequence to only emit even integers. This example replaces the Subscribers.Sink subscriber with a `for`-`await`-`in` loop that iterates over the AsyncPublisher provided by the `values` property.

```
let numbers: [Int] = [1, 2, 3, 4, 5]
let filtered = numbers.publisher
    .filter { $0 % 2 == 0 }

for await number in filtered.values
{
    print("\(number)", terminator: " ")
}
```

