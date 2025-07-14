

- InputMethodKit
- IMKStateSetting
-  setValue(\_:forTag:client:) 

Instance Method

# setValue(\_:forTag:client:)

Set the value for the provided key.

macOS 10.5+

``` source
func setValue(
    _ value: Any!,
    forTag tag: Int,
    client sender: Any!
)
```

**Required**

## Parameters 

`value`  

The value, specified as the appropriate object (such as `NSNumber`), to set.

`tag`  

The key whose value you want to set.

`sender`  

The client setting the value.

## See Also

### Getting and Setting Values

func value(forTag: Int, client: Any!) -> Any!

Returns a value object whose key is the provided tag.

**Required**

