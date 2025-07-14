

- Foundation
- UserDefaults
-  removeObject(forKey:) 

Instance Method

# removeObject(forKey:)

Removes the value of the specified default key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeObject(forKey defaultName: String)
```

## Parameters 

`defaultName`  

The key whose value you want to remove.

## Discussion

Removing a default has no effect on the value returned by the object(forKey:) method if the same key exists in a domain that precedes the standard application domain in the search list.

## See Also

### Related Documentation

func set(Any?, forKey: String)

Sets the value of the specified default key.

