

- AdAttributionKit
- AppImpression
-  sourceID 

Instance Property

# sourceID

A four-digit integer that ad networks define to represent the ad campaign.

iOS 17.4+iPadOS 17.4+Mac Catalyst

``` source
var sourceID: Int { get }
```

## Discussion

The `sourceID` is also known as the *hierarchical source identifier*. Ad networks and developers define its meaning. This integer can have up to four digits. You might receive two, three, or all four digits of the `sourceID` in the first winning postback, based on the data tier of the postback. You can use the different digits of the source identifier to represent different aspects of your ad, such as campaign information, placement, locale, and so on. For more information about the values you might get in the postback, see Identifying the parameters in a postback.

Note

A postback report represents this integer as a string in the `source-identifier` parameter in the payload of the JSON Web Signature (JWS). For more details about the parameters of a postback, see Identifying the parameters in a postback.

