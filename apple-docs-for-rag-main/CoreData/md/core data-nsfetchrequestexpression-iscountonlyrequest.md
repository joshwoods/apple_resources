

- Core Data
- NSFetchRequestExpression
-  isCountOnlyRequest 

Instance Property

# isCountOnlyRequest

Returns a Boolean value that indicates whether the receiver represents a count-only fetch request.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var isCountOnlyRequest: Bool { get }
```

## Discussion

true if the receiver represents a count-only fetch request, otherwise false. If this method returns false, the managed object context (from the contextExpression) will perform fetch(_:): with the requestExpression; if this method returns true, the managed object context will perform count(for:) with the requestExpression.

## See Also

### Examining a Fetch Request Expression

var requestExpression: NSExpression

The expression for the receiver’s fetch request.

var contextExpression: NSExpression

The expression for the receiver’s managed object context.

