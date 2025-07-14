

- Open Directory
- ODNode
-  supportedRecordTypes() 

Instance Method

# supportedRecordTypes()

Returns an array of the record types supported by the node.

Mac CatalystmacOS 10.6+

``` source
func supportedRecordTypes() throws -> [Any]
```

## Return Value

An array of supported record types.

## Discussion

If the node does not support checking for supported record types, all possible record types are returned.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Managing Node Records

func createRecord(withRecordType: String!, name: String!, attributes: [AnyHashable : Any]!) throws -> ODRecord

Creates a record in a specified node with specified properties.

func record(withRecordType: String!, name: String!, attributes: Any!) throws -> ODRecord

Returns a record from the node with a specified type and name.

func supportedAttributes(forRecordType: String!) throws -> [Any]

Returns an array of attribute types supported by the node’s records.

