

- Quartz
- QCPlugIn
-  setSerializedValue(\_:forKey:) Deprecated

Instance Method

# setSerializedValue(\_:forKey:)

Provides custom deserialization for patch internal settings that were previously serialized using the method serializedValue(forKey:).

macOS 10.4–10.15Deprecated

``` source
func setSerializedValue(
    _ serializedValue: Any!,
    forKey key: String!
)
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`serializedValue`  

The value to deserialize.

`key`  

The key for the value to deserialize.

## Discussion

If your patch has internal settings that do not conform to the NSCoding protocol, you must implement this method. After you deserialize the value, you need to call `[self set:value forKey:key]` to set the corresponding internal setting of the custom patch instance to the deserialized value.

## See Also

### Supporting Saving and Retrieving Internal Settings

func serializedValue(forKey: String!) -> Any!

A method implemented to override serialization.

Deprecated

