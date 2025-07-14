

- PassKit (Apple Pay and Wallet)
- PKIdentityElement
-  age(atLeast:) 

Type Method

# age(atLeast:)

Returns an element that represents the user’s age is at least the age you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
class func age(atLeast age: Int) -> Self
```

## Parameters 

`age`  

The age a user must at least be, in years from `1` to `125`.

## Return Value

An instance with the age you specify if the user’s age is at least the age you specify. If the element is unavailable, this method falls back to a request for age.

## Mentioned in 

Requesting identity data from a Wallet pass

## See Also

### Getting an age identity element

class var age: PKIdentityElement

An element that represents the user’s age, in years.

