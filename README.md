# Google Places (google-places)

The Google Places API is a service that accepts HTTP requests for location data through a variety of methods. It returns formatted location data and imagery about establishments, geographic locations, or prominent points of interest. Supports nearby search, text search, place details, place photos, and autocomplete.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/google-places/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Restaurant, Geolocation, Google, Locations, Maps, Places, Points of Interest

## Timestamps

- **Created:** 2026-03-13
- **Modified:** 2026-06-02

## APIs

### Google Places API

The Places API (New) provides programmatic access to Google's database of places, including establishments, geographic locations, and points of interest. It supports nearby search, text search, place details, photos, and autocomplete predictions.

**Human URL:** [https://developers.google.com/maps/documentation/places/web-service](https://developers.google.com/maps/documentation/places/web-service)

#### Tags:

 - Locations, Maps, Places, Search

#### Properties

- [OpenAPI](openapi/openapi.yml)
- [JSONSchema](json-schema/Place.json)
- [NaftikoCapability — Search](capabilities/openapi-search.yaml)
- [NaftikoCapability — Places](capabilities/openapi-places.yaml)
- [Android SDK](https://developers.google.com/maps/documentation/places/android-sdk/overview)
- [iOS SDK](https://developers.google.com/maps/documentation/places/ios-sdk/overview)
- [JavaScript Library](https://developers.google.com/maps/documentation/javascript/places)
- [Node.js Client](https://www.npmjs.com/package/@googlemaps/google-maps-services-js)
- [Python Client](https://pypi.org/project/googlemaps/)
- [Java Client](https://github.com/googlemaps/google-maps-services-java)
- [JavaScript Samples](https://github.com/googlemaps/js-samples)
- [Documentation](https://developers.google.com/maps/documentation/places/web-service)

## Common Properties

- [GitHubOrganization](https://github.com/googlemaps)
- [Tools — MCP Server](https://github.com/googlemaps/platform-ai)
- [Tools — MCP Server (Grounding)](https://developers.google.com/maps/ai/grounding-lite/reference/mcp)
- [GettingStarted](https://developers.google.com/maps/documentation/places/web-service/overview)
- [Authentication](https://developers.google.com/maps/documentation/places/web-service/get-api-key)
- [Pricing](https://developers.google.com/maps/billing-and-pricing/pricing)
- [RateLimits](rate-limits/google-places-rate-limits.yml)
- [Plans](plans/google-places-plans-pricing.yml)
- [FinOps](finops/google-places-finops.yml)
- [JSONLD](json-ld/context.jsonld)
- [Spectral](rules/google-places-spectral-rules.yml)
- [Vocabulary](vocabulary/google-places-vocabulary.yml)
- [SupportTermsOfService](https://cloud.google.com/maps-platform/terms)

## Features

| Name | Description |
|------|-------------|
| Text Search | Search for places using free-form text queries such as "pizza near Boston" and return matching establishments and points of interest. |
| Nearby Search | Find places within a specified geographic radius, optionally filtered by place type, ranked by distance or prominence. |
| Place Details | Retrieve comprehensive information about a place including address, opening hours, ratings, reviews, contact details, and photos. |
| Place Photos | Access high-quality photographic content associated with a place from Google's database. |
| Autocomplete | Return place and query predictions in response to partial text input, with optional session-based billing. |

## Use Cases

| Name | Description |
|------|-------------|
| Location Discovery | Help users discover restaurants, hotels, and points of interest near their current location. |
| Address Autocomplete | Provide type-ahead address and place suggestions in forms to reduce input errors and speed up checkout flows. |
| Delivery Enrichment | Enrich delivery and logistics status updates with verified place details and geolocation data. |
| Travel and Tourism | Show travelers establishment contact information, pricing signals, reviews, ratings, and photos. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Google Places API (New)](openapi/openapi.yml)

### JSON Schema

16 generated schemas plus a hand-crafted Place schema in [json-schema/](json-schema/), including `place-schema.json`, `review-schema.json`, `photo-schema.json`, `opening-hours-schema.json`, `lat-lng-schema.json`, and the request/response schemas for search and autocomplete.

### JSON Structure

16 JSON Structure documents in [json-structure/](json-structure/) mirroring the JSON Schema set.

### JSON-LD

- [Google Places Context (hand-crafted)](json-ld/context.jsonld)
- [Google Places API Context (generated)](json-ld/google-places-api-context.jsonld)

### Examples

16 example payloads in [examples/](examples/), one per schema.

## Capabilities

Naftiko capabilities, one self-contained file per OpenAPI tag, each exposing both a REST and an MCP adapter routed through an inline consumes block.

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Search](capabilities/openapi-search.yaml) | Google Places API | 3 | Application Developer, Search Integrator |
| [Places](capabilities/openapi-places.yaml) | Google Places API | 2 | Application Developer, Content Enrichment Engineer |

## Vocabulary

- [Google Places Vocabulary](vocabulary/google-places-vocabulary.yml) — Unified taxonomy mapping 2 resources, 3 actions, 2 workflows, and 3 personas across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [Google Places Spectral Rules](rules/google-places-spectral-rules.yml) — 39 rules across 13 categories enforcing Google Places API conventions

## Commercial

- [Plans & Pricing](plans/google-places-plans-pricing.yml) — Pay-as-you-go per-SKU pricing across Essentials, Pro, and Enterprise tiers (API Commons Plans 0.1)
- [Rate Limits](rate-limits/google-places-rate-limits.yml) — Per-method per-minute project quotas (API Commons Rate Limits 0.1)
- [FinOps](finops/google-places-finops.yml) — FOCUS-aligned usage-based billing model (FinOps Framework 1.0)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
