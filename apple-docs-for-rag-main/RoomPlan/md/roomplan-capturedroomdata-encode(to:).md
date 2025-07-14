

- RoomPlan
- CapturedRoomData
-  encode(to:) 

Instance Method

# encode(to:)

Serializes captured room data to the specified encoder.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func encode(to encoder: any Encoder) throws
```

## Parameters 

`encoder`  

An object that the captured room data serializes to.

## Discussion

An app might serialize a CapturedRoomData object to defer processing to a later date or to defer processing to another device.

