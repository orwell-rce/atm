#GPS

## Package.
The main Namespace is com.progress.demo.rce.gps

## Events.

* **NewPOI**(integer id, string name, location pos). It register a new Point Of Interest with its id, name and its location .
* **NewSim**(integer id, float limX, float limY). It defines a new random-walk simulator for the id-client; limX represents the maximum x-axis value and analogous for the limY.
* **Position**(integer id, location pos). This is the actual client position.
* **Stream**(string channel, integer idChannel, integer idClient, sequence<string> extra). The output event that has the information about the channel, its id, the client id and the extra information.
In this case, the channel is "GPS", and extra = [POI-location, Client-location].


