

- Open Directory
- ODRecord
-  recordType 

Instance Property

# recordType

The record’s type.

Mac CatalystmacOS 10.6+

``` source
var recordType: String! { get }
```

## See Also

### Managing Record Attributes

func addValue(Any!, toAttribute: String!) throws

Adds a value to an attribute of the record.

func recordDetails(forAttributes: [Any]!) throws -> [AnyHashable : Any]

Returns a dictionary of attributes with their respective values.

var recordName: String!

The official name of the record.

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

