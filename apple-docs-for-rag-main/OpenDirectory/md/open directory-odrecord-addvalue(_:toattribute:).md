

- Open Directory
- ODRecord
-  addValue(\_:toAttribute:) 

Instance Method

# addValue(\_:toAttribute:)

Adds a value to an attribute of the record.

Mac CatalystmacOS 10.6+

``` source
func addValue(
    _ inValue: Any!,
    toAttribute inAttribute: String!
) throws
```

## Parameters 

`inValue`  

The value. Should be of type `NSString` or `NSData`.

`inAttribute`  

The attribute.

## Discussion

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Managing Record Attributes

func recordDetails(forAttributes: [Any]!) throws -> [AnyHashable : Any]

Returns a dictionary of attributes with their respective values.

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

