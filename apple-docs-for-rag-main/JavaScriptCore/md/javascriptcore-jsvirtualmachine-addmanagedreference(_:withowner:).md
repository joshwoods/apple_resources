

- JavaScriptCore
- JSVirtualMachine
-  addManagedReference(\_:withOwner:) 

Instance Method

# addManagedReference(\_:withOwner:)

Notifies the JavaScriptCore virtual machine of an external object relationship.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func addManagedReference(
    _ object: Any!,
    withOwner owner: Any!
)
```

## Parameters 

`object`  

The object to be referenced by the JavaScript memory management graph.

`owner`  

The other object responsible for the lifetime of the reference.

## Discussion

Use this method to make the JavaScript runtime aware of arbitrary external Objective-C or Swift object graphs. The runtime can then use this information to retain any JavaScript values that are referenced from somewhere in said object graph.

For correct behavior, clients must make their external object graphs reachable from within the JavaScript runtime. If an Objective-C or Swift object is reachable from within the JavaScript runtime, all managed references transitively reachable from it as recorded using the addManagedReference(_:withOwner:) method are scanned by the garbage collector.

## See Also

### Managing Memory for Bridged Values

func removeManagedReference(Any!, withOwner: Any!)

Notifies the JavaScriptCore virtual machine that a previously registered object relationship no longer exists.

