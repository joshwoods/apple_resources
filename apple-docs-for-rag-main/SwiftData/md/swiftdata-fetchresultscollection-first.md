

- SwiftData
- FetchResultsCollection
-  first 

Instance Property

# first

The first element of the collection.

SwiftDataSwiftiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var first: Self.Element? { get }
```

## Discussion

If the collection is empty, the value of this property is `nil`.

```
let numbers = [10, 20, 30, 40, 50]
if let firstNumber = numbers.first {
    print(firstNumber)
}
// Prints "10"
```

