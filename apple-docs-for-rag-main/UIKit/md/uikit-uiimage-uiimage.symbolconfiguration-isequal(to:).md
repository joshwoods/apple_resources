

- UIKit
- UIImage
- UIImage.SymbolConfiguration
-  isEqual(to:) 

Instance Method

# isEqual(to:)

Returns a Boolean value that indicates whether the configuration objects are equivalent.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func isEqual(to otherConfiguration: UIImage.SymbolConfiguration?) -> Bool
```

## Parameters 

`otherConfiguration`  

The other configuration object. Specify `nil` to compare the current configuration object to the configuration object in the unspecified property.

## Return Value

true if the trait collections and image configuration values of both objects match; otherwise, false.

