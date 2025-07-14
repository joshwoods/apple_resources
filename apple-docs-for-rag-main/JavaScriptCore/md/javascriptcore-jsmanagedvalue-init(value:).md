

- JavaScriptCore
- JSManagedValue
-  init(value:) 

Initializer

# init(value:)

Initializes a managed value with the specified JavaScript value.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
init!(value: JSValue!)
```

## Parameters 

`value`  

A JavaScript value.

## Return Value

A new managed value.

## Discussion

To ensure that the underlying JavaScript value is retained as long as the managed value remains in use in the Objective-C or Swift runtime, report the managed value’s owner to the JavaScriptCore virtual machine using the addManagedReference(_:withOwner:) method.

## See Also

### Creating a Managed Value

init!(value: JSValue!, andOwner: Any!)

Creates a managed value and associates it with an owner.

