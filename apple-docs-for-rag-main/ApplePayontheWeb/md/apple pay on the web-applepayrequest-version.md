

- Apple Pay on the Web
- ApplePayRequest
-  version 

Instance Property

# version

The Apple Pay version supported on your website.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
required long version;
```

## Discussion

The version number you provide here represents the minimum Apple Pay version that the user’s browser must support. You can check which API version the browser supports by calling supportsVersion.

Always check supportsVersion before using an Apple Pay feature that isn’t available in all versions. See Apple Pay on the web version history for information about the features available in each version.

## See Also

### Identifier and version information

merchantIdentifier

The merchant identifier you registered with Apple for use with Apple Pay.

