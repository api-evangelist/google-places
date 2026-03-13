# Google Places API

The Google Places API is a service that accepts HTTP requests for location data through a variety of methods. It returns formatted location data and imagery about establishments, geographic locations, or prominent points of interest.

## APIs

- **Google Places API (New)** - Provides programmatic access to Google's database of places including nearby search, text search, place details, photos, and autocomplete.

## Base URL

```
https://places.googleapis.com/v1
```

## Key Endpoints

- **Nearby Search** - `POST /places:searchNearby` - Search for places near a location
- **Text Search** - `POST /places:searchText` - Search for places using text queries
- **Place Details** - `GET /places/{placeId}` - Get details about a specific place
- **Place Photos** - `GET /places/{placeId}/photos/{photoReference}/media` - Get place photos
- **Autocomplete** - `POST /places:autocomplete` - Get place predictions

## Artifacts

- [APIs.yml](apis.yml) - APIs.json index
- [OpenAPI](openapi/openapi.yml) - OpenAPI 3.1.0 specification
- [JSON Schema](json-schema/Place.json) - JSON Schema (draft 2020-12) for Place
- [JSON-LD Context](json-ld/context.jsonld) - JSON-LD context mapping

## Resources

- [Getting Started](https://developers.google.com/maps/documentation/places/web-service/overview)
- [Pricing](https://developers.google.com/maps/billing-and-pricing/pricing)
- [API Reference](https://developers.google.com/maps/documentation/places/web-service)

## Maintainers

- **Kin Lane** - kin@apievangelist.com
