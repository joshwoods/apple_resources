

- Foundation
- UserDefaults
-  synchronize() 

Instance Method

# synchronize()

Waits for any pending asynchronous updates to the defaults database and returns; this method is unnecessary and shouldn’t be used.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func synchronize() -> Bool
```

## Return Value

true if the data was saved successfully to disk, otherwise false.

## See Also

### Related Documentation

func removePersistentDomain(forName: String)

Removes the contents of the specified persistent domain from the user’s defaults.

func persistentDomain(forName: String) -> [String : Any]?

Returns a dictionary representation of the defaults for the specified domain.

func setPersistentDomain([String : Any], forName: String)

Sets a dictionary for the specified persistent domain.

### Legacy

convenience init?(user: String)

Creates a user defaults object initialized with the defaults for the specified user account.

Deprecated

class func resetStandardUserDefaults()

This method has no effect and shouldn’t be used.

Language-Dependent Information Constants

These constants are deprecated and shouldn’t be used.

