

- JavaScriptCore
- JSManagedValue
-  init(value:andOwner:) 

Initializer

# init(value:andOwner:)

Creates a managed value and associates it with an owner.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
init!(
    value: JSValue!,
    andOwner owner: Any!
)
```

## Parameters 

`value`  

A JavaScript value.

`owner`  

The Objective-C or Swift object responsible for

## Return Value

A new managed value.

## Discussion

Calling this method is equivalent to creating a managed value and then reporting it to the JavaScriptCore virtual machine using the addManagedReference(_:withOwner:) method.

## See Also

### Creating a Managed Value

init!(value: JSValue!)

Initializes a managed value with the specified JavaScript value.

