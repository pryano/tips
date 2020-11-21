# Time
Time is trickier than you'd think and is rarely covered in much detail in school. 
But timezones, time-parsing, or time-keeping crop up in almost every application. 
Here are some things that you have no reason to know if you're fresh out of school.

## Monotonic Time
Generally when you want to track duration in your code, you should use a `monotonic` timer.
A monotonic timer is one that increments in one direction. It will not be affected by daylight savings time, leap seconds, or changes in time servers.
Every language I've used has a built-in monotonic timer in its time library.

## Daylight Savings Time
Sometimes modifying your code to accomodate DST is not worth the time it takes to implement. 
Sometimes it's easier to restart your process twice a year.
Determine if anything could be affected on those 2 occasions in the year and if it's okay for them to error.

## Daylight Savings Time 2
In general, never try to handle DST or time zones yourself, always lean on a library. Time zones are incredibly complicated with a lot of edge cases.
Make sure you also keep your library version up to date, since changes regularly occur.

## Time Zones
Store everything in UFC if you can, and do the timezone conversion on the frontend.
This makes calculations easier because everything is at the same offset.
