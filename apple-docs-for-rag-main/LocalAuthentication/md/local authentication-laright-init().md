

- Local Authentication
- LARight
-  init() 

Initializer

# init()

Creates a right using the default authorization requirements.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
init()
```

## See Also

### Authorizing a right

init(requirement: LAAuthenticationRequirement)

Creates a right with the authentication requirements you supply.

var tag: Int

An integer you use to identify a right.

func authorize(localizedReason: String, completion: ((any Error)?) -> Void)

Performs an authorization on the right.

func authorize(localizedReason: String, in: LAPresentationContext, completion: ((any Error)?) -> Void)

Performs an authorization on the right with a window context you supply.

