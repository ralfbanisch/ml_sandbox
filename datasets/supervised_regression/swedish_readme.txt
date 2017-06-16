This data is courtesy of Prof. Nikki Vercauteeren. It can be used to build
a model for e.g. predicting temperature based on different features of the
geographical location. The .m file contains more information
plus routines for extracting (sorry, no python conversion here).

There is for 64 locations:


-
ID = Loggers{1,1};          %Number identity of the logger (vercauteren's map)
Name = Loggers{1,2};        % Name of the hill
Lat = Loggers{1,3};         %latitude
Long = Loggers{1,4};        %longitude
Orientation = Loggers{1,5}; %north, south, east or west facing
DistanceSea = Loggers{1,6}; %approximate distance to the shore
Elevation = Loggers{1,7};   %approximate elevation in m

additionally, for one year, hourly frequency:

- air temperature, at 1m every hour
- ground temperature, just under a moss cover, every hour
- corresponding time vector (matlab time)

and insolation, monthly, for every month and every location (how to extract them is in the .m file)
