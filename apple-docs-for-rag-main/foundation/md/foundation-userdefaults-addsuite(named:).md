

- Foundation
- UserDefaults
-  addSuite(named:) 

Instance Method

# addSuite(named:)

Inserts the specified domain name into the receiver’s search list.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addSuite(named suiteName: String)
```

## Parameters 

`suiteName`  

The domain name to insert.

## Discussion

The `suiteName` domain is similar to a bundle identifier string, but isn’t necessarily tied to a particular application or bundle. A suite can be used to hold preferences that are shared between multiple applications.

The additional search lists of the `suiteName` domain are searched after the current domain, but before global defaults (that is, when a suite is added, the preferences subsystem first searches the app’s user preferences, then searches again as though it were an app with a bundle identifier equal to `suiteName`, and then finally searches the global preferences). Passing globalDomain or the current application’s bundle identifier is unsupported.

## See Also

### Related Documentation

class var standard: UserDefaults

Returns the shared defaults object.

### Maintaining Suites

func removeSuite(named: String)

Removes the specified domain name from the receiver’s search list.

