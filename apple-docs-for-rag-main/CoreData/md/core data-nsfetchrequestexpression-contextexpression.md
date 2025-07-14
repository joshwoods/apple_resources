

- Core Data
- NSFetchRequestExpression
-  contextExpression 

Instance Property

# contextExpression

The expression for the receiver’s managed object context.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var contextExpression: NSExpression { get }
```

## Discussion

The expression must evaluate to an NSManagedObjectContext object.

## See Also

### Examining a Fetch Request Expression

var requestExpression: NSExpression

The expression for the receiver’s fetch request.

var isCountOnlyRequest: Bool

Returns a Boolean value that indicates whether the receiver represents a count-only fetch request.

