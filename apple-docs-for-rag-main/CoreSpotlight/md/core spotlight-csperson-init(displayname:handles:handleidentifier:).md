

- Core Spotlight
- CSPerson
-  init(displayName:handles:handleIdentifier:) 

Initializer

# init(displayName:handles:handleIdentifier:)

Returns a new `CSPerson` object initialized with the specified display name and contact attributes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
init(
    displayName: String?,
    handles: [String],
    handleIdentifier: String
)
```

## Parameters 

`displayName`  

The name of the person in a user-displayable string.

`handles`  

An array of contact handles, such as phone number or email address.

`handleIdentifier`  

A property key that specifies a handle type, such as CNContactEmailAddressesKey.

## Return Value

An initialized person object that represents a user’s contact.

