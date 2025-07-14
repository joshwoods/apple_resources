

- Local Authentication
- LARight
-  tag 

Instance Property

# tag

An integer you use to identify a right.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var tag: Int { get set }
```

## See Also

### Authorizing a right

init()

Creates a right using the default authorization requirements.

init(requirement: LAAuthenticationRequirement)

Creates a right with the authentication requirements you supply.

func authorize(localizedReason: String, completion: ((any Error)?) -> Void)

Performs an authorization on the right.

func authorize(localizedReason: String, in: LAPresentationContext, completion: ((any Error)?) -> Void)

Performs an authorization on the right with a window context you supply.

