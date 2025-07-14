

- Foundation
- UserDefaults
-  set(\_:forKey:) 

Instance Method

# set(\_:forKey:)

Sets the value of the specified default key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func set(
    _ value: Any?,
    forKey defaultName: String
)
```

## Parameters 

`value`  

The object to store in the defaults database.

`defaultName`  

The key with which to associate the value.

## Discussion

The `value` parameter can be only property list objects: NSData, NSString, NSNumber, NSDate, NSArray, or NSDictionary. For NSArray and NSDictionary objects, their contents must be property list objects. For more information, see What is a Property List? in Property List Programming Guide.

Setting a default has no effect on the value returned by the object(forKey:) method if the same key exists in a domain that precedes the application domain in the search list.

## See Also

### Related Documentation

func removeObject(forKey: String)

Removes the value of the specified default key.

### Setting Default Values

func set(Float, forKey: String)

Sets the value of the specified default key to the specified float value.

func set(Double, forKey: String)

Sets the value of the specified default key to the double value.

func set(Int, forKey: String)

Sets the value of the specified default key to the specified integer value.

func set(Bool, forKey: String)

Sets the value of the specified default key to the specified Boolean value.

func set(URL?, forKey: String)

Sets the value of the specified default key to the specified URL.

