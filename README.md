# Mobile Traffic Simulator (Matlab) version 1.0
The simulator creates bursty raw data traffic according to mobile usage characteristics. It produces... 
- uplink and downlink data volumes for 
- an arbitrary number of users (~ up to 2.500) 
- in freely chosen time intervals (from several minutes to several days)
- at arbitrary interval sizes (1m to 1hour)
- comes with exemplary models for weekday and weekend traffic patterns.
- Patterns are derived from traffic measurements 

The generator is designed to produce self-similar traffic. A modulated Poisson Process  (-> number of bursts per increment) is combined with a random burst size generator (-> size per burst). Burst sizes are simulated by the pareto distribution. The intensity of the Poisson process (lambda parameter) is modulated by so called native activity pattterns (NAPs) representing the distribution of upload (and download activity) of characteristic user typs oder daytime. 

The exemplary models (current_model) can be altered by replacing them by new files which must have the same data structure.

Usage:
1. Unzip the archive into a folder an open in Matlab.
2. Start the MTS_config file.
3. Change Parameters as desired.

Annotations:
- The model is intended to produce plausible results without requiring intensive preparation / setup effort. It does not consider any protocols.
- It is derived "top-down" from mobile traffic measurements and can be enhanced by more detailed measurements 
- The output is to be consideres as "raw traffic", i.e. no device (processing) limitations, rate limits or volume caps have been considered. 

More on the theoretical backgound you can find under: LINK after publishing 
