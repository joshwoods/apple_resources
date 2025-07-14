

- Apple Maps Server API
- EtaResponse
-  EtaResponse.Eta 

Object

# EtaResponse.Eta

An object that contains details about an estimated time of arrival (ETA).

Apple Maps Server API 1.2+

``` source
object EtaResponse.Eta
```

## Properties

`destination`

Location

The destination as a Location.

`distanceMeters`

`integer`

The distance in meters to the destination.

`expectedTravelTimeSeconds`

`integer`

The estimated travel time in seconds, including delays due to traffic.

`staticTravelTimeSeconds`

`integer`

The expected travel time, in seconds, without traffic.

`transportType`

`string`

A string that represents the mode of transportation for this ETA, which is one of:

- Automobile

- Transit

- Walking

Possible Values: `Automobile, Transit, Walking`

