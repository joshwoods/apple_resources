

- Address Book
-  ABImageClient 

Protocol

# ABImageClient

Methods for responding to a request to load images associated with a contact.

macOS

``` source
protocol ABImageClient : NSObjectProtocol
```

## Topics

### Loading an image

func consumeImageData(Data!, forTag: Int)

Gets the image data for the given tag that was initiated by an asynchronous fetch.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Data Types

class ABPerson

An object that encapsulates all information about a person in the Address Book database.

class ABGroup

An object that represents a group of records in the Address Book database.

class ABMultiValue

An immutable representation of a property that might have multiple values.

class ABMutableMultiValue

A mutable representation of a property that might have multiple values.

class ABRecord

An abstract class that defines the common properties for all Address Book records.

