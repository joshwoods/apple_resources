

- ProximityReader
- VASRequest
-  localizedVASType 

Instance Property

# localizedVASType

The localized name of the loyalty program.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
final let localizedVASType: String
```

## Discussion

Specify the loyalty program name, instead of a payment amount, when you request only a Value Added Services (VAS) read. The maximum length of this string is 22 characters.

## See Also

### Getting the loyalty card details

let vasMerchants: [VASRequest.Merchant]

The list of merchants to match against the user’s Wallet content or loyalty card.

struct Merchant

The identity of a merchant that offers a loyalty program.

