# SAMP Timelapse

Timelapse Function - Easy to use

## Function

```pawn
// Function
GetTimelapse(start, end)
IsTimePassed(time)
```

## Example How to use

GetTimelapse

```pawn
#include "P_Timelapse.inc"

main ()
{
    new var = gettime() + 60, // var is 60 seconds
        var2 = gettime() + 120; // var2 is 120 seconds

    printf("%s", GetTimelapse(var, var2));
    // This thing will print gap between 2 UNIX timestamp (var & var2)
}
````

IsTimePassed

```pawn
#include "P_Timelapse.inc"

main ()
{
    new var = gettime() + 5;
    printf("%s", (IsTimepassed(var)) ? ("Passed") : ("Not Passed");
    // This thing will print is Time passed or not
}
````
