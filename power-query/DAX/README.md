#Total Snowfall
```Total Snowfall =
SUM(SnowOperations[Snowfall_cm])
```
#Number of Snowfall Events
```Number of Snowfall Events =
DISTINCTCOUNT(SnowOperations[SnowEventID])
```
#Total Labor Hours
```Total Labor Hours =
SUM(SnowOperations[LaborHours])
```
#Heaviest Snowfall
```Heaviest Snowfall =
MAX(SnowOperations[Snowfall_cm])
```
#Total Event Cost
```Total Event Cost =
SUM(SnowOperations[EventCost])
```
#Completed Events
```Completed Events =
CALCULATE(
    DISTINCTCOUNT(SnowOperations[SnowEventID]),
    SnowOperations[Status] = "Completed"
)
```
#Completion %
```Completion % =
DIVIDE(
    [Completed Events],
    [Number of Snowfall Events],
    0
)
```
