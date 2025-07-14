

- Metal
- MTLStructType
-  memberByName(\_:) 

Instance Method

# memberByName(\_:)

Provides a representation of a struct member.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func memberByName(_ name: String) -> MTLStructMember?
```

## Parameters 

`name`  

The name of a member in the struct.

## Return Value

An object that represents the named struct member. If `name` does not match a member name, `nil` is returned.

## See Also

### Obtaining Information about Struct Members

var members: [MTLStructMember]

An array of objects that describe the fields in the struct.

