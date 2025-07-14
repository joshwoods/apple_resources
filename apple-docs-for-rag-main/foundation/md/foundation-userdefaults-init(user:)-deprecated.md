

- Foundation
- UserDefaults
-  init(user:) Deprecated

Initializer

# init(user:)

Creates a user defaults object initialized with the defaults for the specified user account.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
convenience init?(user username: String)
```

Deprecated

This method was never implemented to return anything but the defaults for the current user. Use standard instead.

## Parameters 

`username`  

The name of the user account.

## Return Value

An initialized UserDefaults object whose argument and registration domains are already set up. If the current user does not have access to the specified user account, this method returns `nil`.

## Discussion

This method doesn’t put anything in the search list. Invoke it only if you’ve allocated your own UserDefaults instance instead of using the shared one.

You do not normally use this method to initialize an instance of UserDefaults. Applications used by a superuser might use this method to update the defaults databases for a number of users. The user who started the application must have appropriate access (read, write, or both) to the defaults database of the new user, or this method returns `nil`.

### Special Considerations

This method was never implemented to do anything except return the defaults for the current user.

## See Also

### Related Documentation

class var standard: UserDefaults

Returns the shared defaults object.

### Legacy

func synchronize() -> Bool

Waits for any pending asynchronous updates to the defaults database and returns; this method is unnecessary and shouldn’t be used.

class func resetStandardUserDefaults()

This method has no effect and shouldn’t be used.

Language-Dependent Information Constants

These constants are deprecated and shouldn’t be used.

