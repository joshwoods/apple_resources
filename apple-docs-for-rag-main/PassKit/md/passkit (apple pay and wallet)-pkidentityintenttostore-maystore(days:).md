

- PassKit (Apple Pay and Wallet)
- PKIdentityIntentToStore
-  mayStore(days:) 

Type Method

# mayStore(days:)

An object that indicates your app may store a data element for the length of time you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
class func mayStore(days: Int) -> Self
```

## Parameters 

`days`  

The length of time to store a data element.

## Return Value

A new instance of PKIdentityIntentToStore.

## Mentioned in 

Requesting identity data from a Wallet pass

