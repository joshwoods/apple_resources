

- Security
- SecCSFlags
-  considerExpiration 

Type Property

# considerExpiration

Consider expired certificates invalid.

Mac Catalyst 13.0+macOS 10.0+

``` source
static var considerExpiration: SecCSFlags { get }
```

## Discussion

When passed to a function that performs code validation, this flag requests that code signatures made by expired certificates be rejected. By default, expiration of participating certificates is not automatic grounds for rejection.

