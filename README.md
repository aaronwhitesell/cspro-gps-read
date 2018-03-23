# GPS read
## Behavior
The ```read``` command will take a new GPS reading. If a new reading within ```gps_desired_accuracy``` cannot be attained in ```max_time``` then the GPS values from any successful read will be used.
## Dictionary variables
Note that *Decimal Char* was set to *Yes* for any value with a decimal part. This states the decimal point will be present in the data file and adds to the length of the numeric.
* Latitude
    * Length: 10
        * Sign: 1
        * Integer part: 2
        * Decimal point: 1
        * Decimal part: 6
            * The sixth decimal place is worth up to 11 cm of granularity
* Longitude
    * Length: 11
        * Sign: 1
        * Integer part: 3
        * Decimal point: 1
        * Decimal part: 6
            * The sixth decimal place is worth up to 11 cm of granularity
* Altitude
    * Length: 7
        * Sign: 1
        * Integer part: 4
        * Decimal point: 1
        * Decimal part: 1
            * The first decimal place is worth up to 10 cm of granularity
* Accuracy
    * Length: 6
        * Integer part: 4
        * Decimal point: 1
        * Decimal part: 1
            * The first decimal place is worth up to 10 cm of granularity
* Satellites
    * Length: 3
        * Integer part: 3
* Readtime
    * Length: 6
        * Integer part: 6
