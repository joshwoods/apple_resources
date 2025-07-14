

- PassKit (Apple Pay and Wallet)
- PKIdentityDocumentDescriptor
-  addElements(\_:intentToStore:) 

Instance Method

# addElements(\_:intentToStore:)

Adds a list of identity element and defines the way an app, or it’s server, stores the elements.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
func addElements(
    _ elements: [PKIdentityElement],
    intentToStore: PKIdentityIntentToStore
)
```

**Required**

## Parameters 

`elements`  

A list of identity elements.

`intentToStore`  

An object that defines how long an app or it’s server stores the elements.

## See Also

### Adding an identity element

class PKIdentityIntentToStore

An object that represents your intention to store an identity element or values derived from an identity element.

