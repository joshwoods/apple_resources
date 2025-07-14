

- InputMethodKit
- IMKStateSetting
-  value(forTag:client:) 

Instance Method

# value(forTag:client:)

Returns a value object whose key is the provided tag.

macOS 10.5+

``` source
func value(
    forTag tag: Int,
    client sender: Any!
) -> Any!
```

**Required**

## Parameters 

`tag`  

The key whose value you want to retrieve.

`sender`  

The client requesting the value.

## Return Value

The value object.

## See Also

### Getting and Setting Values

func setValue(Any!, forTag: Int, client: Any!)

Set the value for the provided key.

**Required**

