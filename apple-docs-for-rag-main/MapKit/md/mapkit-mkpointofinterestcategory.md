

- MapKit
-  MKPointOfInterestCategory 

Structure

# MKPointOfInterestCategory

A point of interest category.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MKPointOfInterestCategory
```

## Topics

### Category creation

init(rawValue: String)

Creates a point of interest category using the provided string.

### Arts and culture

static let museum: MKPointOfInterestCategory

The point of interest category for museums.

static let musicVenue: MKPointOfInterestCategory

The point of interest category for music venues.

static let theater: MKPointOfInterestCategory

The point of interest category for theaters.

### Education

static let library: MKPointOfInterestCategory

The point of interest category for libraries.

static let planetarium: MKPointOfInterestCategory

The point of interest category for planetariums.

static let school: MKPointOfInterestCategory

The point of interest category for schools.

static let university: MKPointOfInterestCategory

The point of interest category for universities.

### Entertainment

static let movieTheater: MKPointOfInterestCategory

The point of interest category for movie theaters.

static let nightlife: MKPointOfInterestCategory

The point of interest category for nightlife.

### Health and safety

static let fireStation: MKPointOfInterestCategory

The point of interest category for fire stations.

static let hospital: MKPointOfInterestCategory

The point of interest category for hospitals.

static let pharmacy: MKPointOfInterestCategory

The point of interest category for pharmacies.

static let police: MKPointOfInterestCategory

The point of interest category for police.

### Historical and cultural landmarks

static let castle: MKPointOfInterestCategory

The point of interest category for castles.

static let fortress: MKPointOfInterestCategory

The point of interest category for fortresses.

static let landmark: MKPointOfInterestCategory

The point of interest category for landmarks.

static let nationalMonument: MKPointOfInterestCategory

The point of interest category for national monuments.

### Food and drink

static let bakery: MKPointOfInterestCategory

The point of interest category for bakeries.

static let brewery: MKPointOfInterestCategory

The point of interest category for breweries.

static let cafe: MKPointOfInterestCategory

The point of interest category for cafes.

static let distillery: MKPointOfInterestCategory

The point of interest category for distilleries.

static let foodMarket: MKPointOfInterestCategory

The point of interest category for food markets, supermarkets, grocery stores, and convenience stores.

static let restaurant: MKPointOfInterestCategory

The point of interest category for restaurants.

static let winery: MKPointOfInterestCategory

The point of interest category for wineries.

### Personal services

static let animalService: MKPointOfInterestCategory

The point of interest category for animal services.

static let atm: MKPointOfInterestCategory

The point of interest category for ATM machines.

static let automotiveRepair: MKPointOfInterestCategory

The point of interest category for automotive repair services.

static let bank: MKPointOfInterestCategory

The point of interest category for banks.

static let beauty: MKPointOfInterestCategory

The point of interest category for beauty services.

static let evCharger: MKPointOfInterestCategory

The point of interest category for EV chargers.

static let fitnessCenter: MKPointOfInterestCategory

The point of interest category for fitness centers.

static let laundry: MKPointOfInterestCategory

The point of interest category for laundries.

static let mailbox: MKPointOfInterestCategory

The point of interest category for mailboxes.

static let postOffice: MKPointOfInterestCategory

The point of interest category for post offices.

static let restroom: MKPointOfInterestCategory

The point of interest category for restrooms.

static let spa: MKPointOfInterestCategory

The point of interest category for spa services.

static let store: MKPointOfInterestCategory

The point of interest category for stores.

### Parks and recreation

static let amusementPark: MKPointOfInterestCategory

The point of interest category for amusement parks.

static let aquarium: MKPointOfInterestCategory

The point of interest category for aquariums.

static let beach: MKPointOfInterestCategory

The point of interest category for beaches.

static let campground: MKPointOfInterestCategory

The point of interest category for campgrounds.

static let fairground: MKPointOfInterestCategory

The point of interest category for fairgrounds.

static let marina: MKPointOfInterestCategory

The point of interest category for marinas.

static let nationalPark: MKPointOfInterestCategory

The point of interest category for national parks.

static let park: MKPointOfInterestCategory

The point of interest category for parks.

static let rvPark: MKPointOfInterestCategory

The point of interest category for recreational vehicle parks.

static let zoo: MKPointOfInterestCategory

The point of interest category for zoos.

### Sports

static let baseball: MKPointOfInterestCategory

The point of interest category for baseball parks.

static let basketball: MKPointOfInterestCategory

The point of interest category for basketball courts.

static let bowling: MKPointOfInterestCategory

The point of interest category for bowling lanes.

static let goKart: MKPointOfInterestCategory

The point of interest category for go-kart services.

static let golf: MKPointOfInterestCategory

The point of interest category for golf courses.

static let hiking: MKPointOfInterestCategory

The point of interest category for hiking areas.

static let miniGolf: MKPointOfInterestCategory

The point of interest category for mini-golf areas.

static let rockClimbing: MKPointOfInterestCategory

The point of interest category for rock-climbing areas.

static let skatePark: MKPointOfInterestCategory

The point of interest category for skate parks.

static let skating: MKPointOfInterestCategory

The point of interest category for skating areas.

static let skiing: MKPointOfInterestCategory

The point of interest category for skiing areas.

static let soccer: MKPointOfInterestCategory

The point of interest category for soccer fields.

static let stadium: MKPointOfInterestCategory

The point of interest category for stadiums.

static let tennis: MKPointOfInterestCategory

The point of interest category for tennis courts.

static let volleyball: MKPointOfInterestCategory

The point of interest category for volleyball courts.

### Travel

static let airport: MKPointOfInterestCategory

The point of interest category for airports.

static let carRental: MKPointOfInterestCategory

The point of interest category for car rentals.

static let conventionCenter: MKPointOfInterestCategory

The point of interest category for convention centers.

static let gasStation: MKPointOfInterestCategory

The point of interest category for gas stations.

static let hotel: MKPointOfInterestCategory

The point of interest category for hotels.

static let parking: MKPointOfInterestCategory

The point of interest category for parking locations.

static let publicTransport: MKPointOfInterestCategory

The point of interest category for locations of public transportation.

### Water sports

static let fishing: MKPointOfInterestCategory

The point of interest category for fishing areas.

static let kayaking: MKPointOfInterestCategory

The point of interest category for kayaking areas.

static let surfing: MKPointOfInterestCategory

The point of interest category for surfing areas.

static let swimming: MKPointOfInterestCategory

The point of interest category for swimming areas.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Points of interest

Identifying unique locations with Place IDs

Obtain information about a point of interest that persists over its lifetime.

class MKMapFeatureAnnotation

A class that describes an annotation element on the map’s display such as a point of interest, territorial boundary, or physical feature.

struct MKMapFeatureOptions

A structure you use to tell the map which kinds of features users can interact with.

class MKMapItemRequest

A utility class you use to request additional information about a map feature.

class MKIconStyle

A class you use to customize the annotation view icon of a point of interest (POI) on the map.

class MKPointOfInterestFilter

A filter that includes or excludes point of interest categories from a map view, local search, or local search completer.

