# Full-Monty integration

This components contains 3 different scripts :

1- Storage

This component acts as a storage for Full Monty components. It reads data in a notecard and make them available to others Full monty scripts.

Please note that there's a syntax to follow :
  - only one "." in the name of the script
  - a number after the ".". This allows the system to deal with multiples notecards
	- the notecard to read must be named "Choregraphy" appended with a "." and a number. A script named "FullMonty-storage-snapshot.0" will read a notecard named "Choregraphy.0". A script named "FullMonty-storage-snapshot.1" will read a notecard named "Choregraphy.1", etc...
	- The storage is configured to deliver its information following these rules
		- ".0" will be delivered to scripts first
		- When ".0" data are all delivered, the script will fall in exhausted mode. ".1" will now deliver its data automatically. And so on. 

2- Integrator

3- Orchestrator