

- Foundation
- StreamSOCKSProxyConfiguration
-  versionKey 

Type Property

# versionKey

Value is either `NSStreamSOCKSProxyVersion4` or `NSStreamSOCKSProxyVersion5`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let versionKey: StreamSOCKSProxyConfiguration
```

## Discussion

If this key is not present, `NSStreamSOCKSProxyVersion5` is used by default.

## See Also

### Type Properties

static let hostKey: StreamSOCKSProxyConfiguration

Value is an `NSString` object that represents the SOCKS proxy host.

static let passwordKey: StreamSOCKSProxyConfiguration

Value is an `NSString` object containing the user’s password.

static let portKey: StreamSOCKSProxyConfiguration

Value is an `NSNumber` object containing an integer that represents the port on which the proxy listens.

static let userKey: StreamSOCKSProxyConfiguration

Value is an `NSString` object containing the user’s name.

