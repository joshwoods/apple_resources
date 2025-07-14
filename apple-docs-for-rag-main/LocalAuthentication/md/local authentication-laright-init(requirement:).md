

- Local Authentication
- LARight
-  init(requirement:) 

Initializer

# init(requirement:)

Creates a right with the authentication requirements you supply.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
init(requirement: LAAuthenticationRequirement)
```

## See Also

### Authorizing a right

init()

Creates a right using the default authorization requirements.

var tag: Int

An integer you use to identify a right.

func authorize(localizedReason: String, completion: ((any Error)?) -> Void)

Performs an authorization on the right.

func authorize(localizedReason: String, in: LAPresentationContext, completion: ((any Error)?) -> Void)

Performs an authorization on the right with a window context you supply.

