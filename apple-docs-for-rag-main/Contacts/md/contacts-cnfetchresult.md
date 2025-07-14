

- Contacts
-  CNFetchResult 

Class

# CNFetchResult

An object that represents the result of a change-history fetch request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
class CNFetchResult where ValueType : AnyObject
```

## Topics

### Accessing results

var currentHistoryToken: Data

An opaque token that indicates a point in history in the user’s Contacts database.

var value: ValueType

The result of the fetch request, expressed as the value type you specify.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Fetch and save requests

class CNContactFetchRequest

An object that defines the options to use when fetching contacts.

class CNFetchRequest

The base class for contact fetch requests.

class CNSaveRequest

An object that collects the changes you want to save to the user’s contacts database.

