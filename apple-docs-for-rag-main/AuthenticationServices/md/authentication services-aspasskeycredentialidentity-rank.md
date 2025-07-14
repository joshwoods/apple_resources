

- Authentication Services
- ASPasskeyCredentialIdentity
-  rank 

Instance Property

# rank

An indicator that enables you to prioritize credential identities relative to each other.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var rank: Int { get set }
```

## Discussion

The system may use the rank to select between credential identities if multiple identities have the same service identifier. A credential identity with a high rank gets precedence over a lower-ranked identity with the same service identifier. The default value is 0.

