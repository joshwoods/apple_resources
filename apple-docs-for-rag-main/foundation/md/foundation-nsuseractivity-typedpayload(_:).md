

- Foundation
- NSUserActivity
-  typedPayload(\_:) 

Instance Method

# typedPayload(\_:)

Decodes the user activity’s user info dictionary as an instance of the specified type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func typedPayload(_ type: T.Type) throws -> T where T : Decodable, T : Encodable
```

## Parameters 

`type`  

The type to decode from userInfo. The `type` must conform to Codable.

## Return Value

The type-safe instance.

## Discussion

Important

This method applies only to SwiftUI apps.

Use this method to retrieve information from the user activity’s userInfo dictionary in a type-safe manner.

If the type can’t be decoded from the userInfo dictionary, this method throws NSUserActivity.TypedPayloadError.invalidContent.

## See Also

### Managing type-safe access to user info

func setTypedPayload&lt;T>(T) throws

Encodes the specified payload into the user activity’s user info dictionary.

enum TypedPayloadError

An enumeration that describes the error types for getting and setting a typed payload.

