

- PassKit (Apple Pay and Wallet)
- PKIdentityDocumentDescriptor
-  intentToStore(element:) 

Instance Method

# intentToStore(element:)

Gets the intent to store for an identity element you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
func intentToStore(element: PKIdentityElement) -> PKIdentityIntentToStore?
```

**Required**

## Parameters 

`element`  

The element to inspect.

## Return Value

A PKIdentityIntentToStore for the element, if available.

