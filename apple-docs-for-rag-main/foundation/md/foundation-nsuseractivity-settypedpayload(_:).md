

- Foundation
- NSUserActivity
-  setTypedPayload(\_:) 

Instance Method

# setTypedPayload(\_:)

Encodes the specified payload into the user activity’s user info dictionary.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func setTypedPayload(_ payload: T) throws where T : Decodable, T : Encodable
```

## Parameters 

`payload`  

The instance to convert to userInfo. The type of the `payload` instance must conform to Codable.

## Discussion

Important

This method applies only to SwiftUI apps.

Use this method to set the user activity’s userInfo dictionary in a type-safe manner. After you set the userInfo dictionary using this approach, the keys in the userInfo dictionary match the coding keys from the Codable type you provide as the `payload`.

If the type can’t be encoded into the userInfo dictionary, this method throws NSUserActivity.TypedPayloadError.encodingError.

## See Also

### Managing type-safe access to user info

func typedPayload&lt;T>(T.Type) throws -> T

Decodes the user activity’s user info dictionary as an instance of the specified type.

enum TypedPayloadError

An enumeration that describes the error types for getting and setting a typed payload.

