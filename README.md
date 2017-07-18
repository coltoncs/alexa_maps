# alexa_maps
A simple node.js script that takes advantage of Amazon Alexa's SDK and Google's Maps API to find directions to a given address from a given destination.

## Requirements
`npm install @google/maps`

`npm install --save alexa-sdk`

## Examples

In order to geocode a location and have the Google Maps API return a RequestHandle.
```
maps.geocode({ 
  address: 'Your address here'
}, function(err, response){
  console.log(response.json.results);
});
```
In order to create a distace matrix given an origin and a destination.
```
maps.distanceMatrix({
  origin: 'Your Origin Address Here',
  destination: 'Your Destination Address Here';
}, function(err, response){
  console.log(response.jsn.results);
});
```

###### Author
*Colton Sweeney* or *pizdetz* on github.
