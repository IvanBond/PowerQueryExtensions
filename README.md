# PowerQueryExtensions
A collection of modules that extend the capabilities of M language (aka Power Query).

## Quickstart
The modules use the extensibility provided by [Data Connectors](https://github.com/Microsoft/DataConnectors), so in order to use them you have to:
1. Copy the the contents of `/build` folder with all the *.mez files onto your local machine
2. Create a `PQ_ExtensionDirectory` environment variable, set its value to this folder
3. Restart Power BI Desktop


## For developers 
In order to extend the modules 
1. Install the [Power Query SDK](https://aka.ms/powerquerysdk) from the Visual Studio Marketplace
2. Edit the existing `Data Connector Projects` or *.pq files 
3. Build the solution
The deployable *.mez files will be located in the Debug folder of each module under `/src`. The Relese configuration of the build will copy these files into the `/build` folder.

## Modules
* [Date](src/Date)
* [List](src/List)
* [Number](src/Number)
* [Splitter](src/Splitter)
* [Table](src/Table)
* [Text](src/Text)
* [Value](src/Value)


## References
The M functions used in this repository have been assembled from a few sources:
* [Power BI Desktop Query Extensions](https://github.com/tnclark8012/Power-BI-Desktop-Query-Extensions)
* [pquery](https://github.com/tycho01/pquery)