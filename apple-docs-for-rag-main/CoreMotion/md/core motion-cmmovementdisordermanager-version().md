

- Core Motion
- CMMovementDisorderManager
-  version() 

Type Method

# version()

Returns a string that describes the movement disorder algorithm’s current version.

watchOS 5.0+

``` source
class func version() -> String?
```

## Mentioned in 

Movement disorder algorithm changelog

## Discussion

Use this method to determine the algorithm used by the movement disorder manager. If the current device supports gathering movement disorder data, this method returns a string with the version number in `..` format. It returns `nil` anytime isAvailable() returns false. For information about the current version, see Movement disorder algorithm changelog.

Important

Your app uses the version of the algorithm provided by the current operating system running on the device. This means the algorithm your app uses might change, without requiring you to rebuild and resubmit your app.

To set up tests that notify you when the version changes, create a unit test that checks the current version against the expected value. You can then use continuous integration to automatically monitor this value with each new release.

```
func testForVersionChange() throws {
    let expectedVersion = "1.0.0"
    let currentVersion = CMMovementDisorderManager.version()
    XCTAssertEqual(expectedVersion, currentVersion, "*** The version has changes to \(String(describing: currentVersion)). ***")
}
```

## See Also

### Checking Availablility

class func isAvailable() -> Bool

A Boolean value indicating whether the current device supports the movement disorder manager.

class func authorizationStatus() -> CMAuthorizationStatus

A value indicating whether the user has authorized the app to monitor and query for movement disorder data.

