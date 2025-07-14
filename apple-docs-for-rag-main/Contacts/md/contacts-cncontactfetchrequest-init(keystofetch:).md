

- Contacts
- CNContactFetchRequest
-  init(keysToFetch:) 

Initializer

# init(keysToFetch:)

Creates a fetch request for the specified keys.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
init(keysToFetch: [any CNKeyDescriptor])
```

## Parameters 

`keysToFetch`  

An array of contact property keys and/or key descriptors from contacts objects to be fetched in the returned contacts. For a list of possible keys, see Contact Keys.

## Return Value

The initialized CNContactFetchRequest instance.

## Discussion

This is the designated initializer for this class. Using `init` raises an exception.

## See Also

### Creating a Fetch Request

protocol CNKeyDescriptor

This protocol is reserved for Contacts framework usage.

