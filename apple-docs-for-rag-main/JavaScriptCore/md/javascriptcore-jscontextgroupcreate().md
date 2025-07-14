

- JavaScriptCore
-  JSContextGroupCreate() 

Function

# JSContextGroupCreate()

Creates a JavaScript context group.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
func JSContextGroupCreate() -> JSContextGroupRef!
```

## Return Value

The created JSContextGroupRef.

## Discussion

A JSContextGroupRef associates JavaScript contexts with one another. Contexts in the same group may share and exchange JavaScript objects. Sharing and exchanging JavaScript objects between contexts in different groups produces undefined behavior. When you use objects from the same context group in multiple threads, explicit synchronization is a requirement.

## See Also

### Creating a Context Group

func JSContextGroupRetain(JSContextGroupRef!) -> JSContextGroupRef!

Retains a JavaScript context group.

func JSContextGroupRelease(JSContextGroupRef!)

Releases a JavaScript context group.

