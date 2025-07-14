

- Open Directory
- ODQuery
-  init(node:forRecordTypes:attribute:matchType:queryValues:returnAttributes:maximumResults:) 

Initializer

# init(node:forRecordTypes:attribute:matchType:queryValues:returnAttributes:maximumResults:)

Creates a query object with provided parameters.

Mac CatalystmacOS 10.6+

``` source
init(
    node inNode: ODNode!,
    forRecordTypes inRecordTypeOrList: Any!,
    attribute inAttribute: String!,
    matchType inMatchType: ODMatchType,
    queryValues inQueryValueOrList: Any!,
    returnAttributes inReturnAttributeOrList: Any!,
    maximumResults inMaximumResults: Int
) throws
```

## Parameters 

`inNode`  

The node to query.

`inRecordTypeOrList`  

The type or types of record to query. Can be an `NSString` object for a single type or an `NSArray` object containing `NSString` objects for multiple types.

`inAttribute`  

The name of the attribute to query.

`inMatchType`  

The type of query.

`inQueryValueOrList`  

The value or values to query in the attribute. Can be an `NSString` object or an `NSData` object for a single value, or an `NSArray` containing `NSString` and `NSData` objects for multiple values.

`inReturnAttributeOrList`  

The attribute or attributes to be returned from the query. Can be an `NSString` object for a single attribute or an `NSArray` object containing `NSString` objects for multiple attributes. Passing `nil` is equivalent to passing `kODAttributeTypeStandardOnly`.

`inMaximumResults`  

The maximum number of values to return.

## Return Value

The initialized query.

## Discussion

Handling Errors in Swift

In Swift, this API is imported as an initializer and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

