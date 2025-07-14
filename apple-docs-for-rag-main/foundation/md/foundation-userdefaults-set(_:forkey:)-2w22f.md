

- Foundation
- UserDefaults
-  set(\_:forKey:) 

Instance Method

# set(\_:forKey:)

Sets the value of the specified default key to the double value.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func set(
    _ value: Double,
    forKey defaultName: String
)
```

## Parameters 

`value`  

The double value.

`defaultName`  

The key with which to associate the value.

## Discussion

This is a convenience method for calling set(_:forKey:).

## See Also

### Setting Default Values

func set(Any?, forKey: String)

Sets the value of the specified default key.

func set(Float, forKey: String)

Sets the value of the specified default key to the specified float value.

func set(Int, forKey: String)

Sets the value of the specified default key to the specified integer value.

func set(Bool, forKey: String)

Sets the value of the specified default key to the specified Boolean value.

func set(URL?, forKey: String)

Sets the value of the specified default key to the specified URL.

