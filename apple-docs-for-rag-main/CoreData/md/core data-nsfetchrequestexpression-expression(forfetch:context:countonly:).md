

- Core Data
- NSFetchRequestExpression
-  expression(forFetch:context:countOnly:) 

Type Method

# expression(forFetch:context:countOnly:)

Returns an expression which will evaluate to the result of executing a fetch request on a context.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func expression(
    forFetch fetch: NSExpression,
    context: NSExpression,
    countOnly countFlag: Bool
) -> NSExpression
```

## Parameters 

`fetch`  

An expression that evaluates to an instance of `NSFetchRequest`.

`context`  

An expression that evaluates to an instance of `NSManagedObjectContext`.

`countFlag`  

If true, when the new expression is evaluated the managed object context (from `context`) will perform count(for:) with the fetch request (from `fetch`). If false, when the new expression is evaluated the managed object context will perform fetch(_:) with the fetch request.

## Return Value

An expression which will evaluate to the result of executing a fetch request (from `fetch`) on a managed object context (from `context`).

## See Also

### Related Documentation

Predicate Programming Guide

Core Data Programming Guide

