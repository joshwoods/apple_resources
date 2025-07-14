

- Foundation
- UserDefaults
-  register(defaults:) 

Instance Method

# register(defaults:)

Adds the contents of the specified dictionary to the registration domain.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func register(defaults registrationDictionary: [String : Any])
```

## Parameters 

`registrationDictionary`  

The dictionary of keys and values you want to register.

## Discussion

If there is no registration domain, one is created using the specified dictionary, and registrationDomain is added to the end of the search list.

The contents of the registration domain are not written to disk; you need to call this method each time your application starts. You can place a plist file in the application’s Resources directory and call register(defaults:) with the contents that you read in from that file.

