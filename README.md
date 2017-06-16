# Mapping

To view maps:
1. download files
2. ensure all files are in the same directory
3. view .html files in RStudio under preview mode

### OR alternatively

Follow steps 1 and 2 above then:
1. install http-server with '$ sudo npm install http-server -g'
2. create a local server with '$  http-server -p 8008 &' 
3. view in browser at localhost:8008
4. note that this method will only allow viewing of 'index.html'

'index.html' refers to a U.S. centered map
'index2.html' refers to a North-America centered map

## Understanding JSON data

Each marker on the map is a feature geometry object in 'us.json'. Within 'us.json', the properties tag under each feature geometry object contains important information for how it is displayed. For now, the 'population' tag corresponds to how large the point will be displayed (i.e. radius). Using the number given in the two objects will preserve identical sizing, although size can be adjusted using larger or smaller numbers. The scaling factor can eventually be altered or outright eliminated as needed, but for now this allows usage of pre-existing code that controls for radius. The 'color' tag contains a string denotation of the color associated with the point. It can be changed to any standard color's string, i.e. "blue", "yello", "orange", etc. This too can eventually be changed as needed, such as containing a different identifier to denote status as current or past member, etc.
