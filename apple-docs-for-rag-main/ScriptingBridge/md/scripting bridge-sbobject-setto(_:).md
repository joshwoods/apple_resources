

- Scripting Bridge
- SBObject
-  setTo(\_:) 

Instance Method

# setTo(\_:)

Sets the receiver to a specified value.

Mac Catalyst 13.0+macOS 10.5+

``` source
func setTo(_ value: Any?)
```

## Parameters 

`value`  

The data the receiver should be set to. It can be an NSString, NSNumber, NSArray, `SBObject`, or any other type of object supported by the Scripting Bridge framework.

## Discussion

You should not call this method directly.

