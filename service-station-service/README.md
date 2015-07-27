# Service Location Service

## Demo Initialization

You can do bulk uploads of location data by POSTing to the `/bulk/serviceLocations` endpoint. E.g.

```
$ curl -H "Content-Type: application/json" localhost:9001/bulk/serviceLocations -d @locations.json
```

where `locations.json` is a file containing a JSON array of `ServiceLocation` objects.
There's a small sample for testing in `src/test/resources`. You can also find
a complete set of US locations at
http://assets.springone2gx2015.s3.amazonaws.com/assets.springone2gx2015/fleet/serviceLocations.json
(available for anonymous download).
