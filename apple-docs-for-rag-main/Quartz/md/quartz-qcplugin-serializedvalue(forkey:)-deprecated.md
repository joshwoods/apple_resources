

- Quartz
- QCPlugIn
-  serializedValue(forKey:) Deprecated

Instance Method

# serializedValue(forKey:)

A method implemented to override serialization.

macOS 10.4–10.15Deprecated

``` source
func serializedValue(forKey key: String!) -> Any!
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`key`  

The key for the value to retrieve.

## Return Value

Either `nil` or a value that’s compliant with property lists: `NSString`, `NSNumber`, `NSDate`, `NSData`, `NSArray`, or `NSDictionary`.

## Discussion

Provides custom serialization for patch internal settings that do not comply to the NSCoding protocol.

## Discussion

If your patch has internal settings that do not conform to the NSCoding protocol, you must implement this method.

## See Also

### Supporting Saving and Retrieving Internal Settings

func setSerializedValue(Any!, forKey: String!)

Provides custom deserialization for patch internal settings that were previously serialized using the method serializedValue(forKey:).

Deprecated

