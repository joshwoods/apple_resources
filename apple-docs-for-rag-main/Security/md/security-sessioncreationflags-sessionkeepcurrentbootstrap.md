

- Security
- SessionCreationFlags
-  sessionKeepCurrentBootstrap 

Type Property

# sessionKeepCurrentBootstrap

The caller has allocated sub-bootstrap.

Mac Catalyst 13.0+macOS 10.0+

``` source
static var sessionKeepCurrentBootstrap: SessionCreationFlags { get }
```

## Discussion

If you create a subset port on your own, you can force

the SessionCreate(_:_:) function to use it by passing this flag in the `flags` parameter. However, you can’t supersede a prior call that way; only a single SessionCreate(_:_:) call is allowed for each session.

