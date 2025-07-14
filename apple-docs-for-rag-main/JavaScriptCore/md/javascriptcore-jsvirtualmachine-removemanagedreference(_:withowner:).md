

- JavaScriptCore
- JSVirtualMachine
-  removeManagedReference(\_:withOwner:) 

Instance Method

# removeManagedReference(\_:withOwner:)

Notifies the JavaScriptCore virtual machine that a previously registered object relationship no longer exists.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func removeManagedReference(
    _ object: Any!,
    withOwner owner: Any!
)
```

## Parameters 

`object`  

The object formerly referenced by the JavaScript memory management graph.

`owner`  

The other object responsible for the lifetime of the reference.

## Discussion

Use this method to deregister object relationships recorded using the addManagedReference(_:withOwner:) method.

The JavaScript garbage collector continues to scan any references that were reported to it until you use this method to remove those references.

## See Also

### Managing Memory for Bridged Values

func addManagedReference(Any!, withOwner: Any!)

Notifies the JavaScriptCore virtual machine of an external object relationship.

