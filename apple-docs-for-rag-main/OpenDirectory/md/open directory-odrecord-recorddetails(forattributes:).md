

- Open Directory
- ODRecord
-  recordDetails(forAttributes:) 

Instance Method

# recordDetails(forAttributes:)

Returns a dictionary of attributes with their respective values.

Mac CatalystmacOS 10.6+

``` source
func recordDetails(forAttributes inAttributes: [Any]!) throws -> [AnyHashable : Any]
```

## Parameters 

`inAttributes`  

An array of attributes. Can be `nil`.

## Return Value

A dictionary of the attributes in `inAttributes` with their respective values.

## Discussion

If `inAttributes` is `nil`, all currently retrieved attributes are returned.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Managing Record Attributes

func addValue(Any!, toAttribute: String!) throws

Adds a value to an attribute of the record.

var recordName: String!

The official name of the record.

var recordType: String!

The record’s type.

func removeValues(forAttribute: String!) throws

Removes all values from an attribute of the record.

func removeValue(Any!, fromAttribute: String!) throws

Removes a value from an attribute of the record.

func setValue(Any!, forAttribute: String!) throws

Sets the values of an attribute of the record.

func synchronize() throws

Synchronizes the record from the directory to get current data and commit changes.

func values(forAttribute: String!) throws -> [Any]

Returns the values of an attribute of the record.

