

- Foundation
- NSCharacterSet
-  urlPasswordAllowed 

Type Property

# urlPasswordAllowed

Returns the character set for characters allowed in a password URL subcomponent.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var urlPasswordAllowed: CharacterSet { get }
```

## Discussion

The password component of a URL is the component immediately following the colon after the username component of the URL, and ends at the `@` sign. For example, in the URL `http://username:password@www.example.com/index.html`, the pass component is `password`.

## See Also

### Getting Character Sets for URL Encoding

class var urlFragmentAllowed: CharacterSet

Returns the character set for characters allowed in a fragment URL component.

class var urlHostAllowed: CharacterSet

Returns the character set for characters allowed in a host URL subcomponent.

class var urlPathAllowed: CharacterSet

Returns the character set for characters allowed in a path URL component.

class var urlQueryAllowed: CharacterSet

Returns the character set for characters allowed in a query URL component.

class var urlUserAllowed: CharacterSet

Returns the character set for characters allowed in a user URL subcomponent.

