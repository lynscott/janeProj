# Process soccer matches

Top Secret Project for Jane ;)

## Usage

Requires Node v12+

Commands:

```.sh
./topTeams input <filepath>
```

or

```
cat <filepath> | ./topTeams
```

## Testing

To run tests execute this from root.

```.sh
./tests
```

## Design

> The basic architecture is a dynamic program that processes
> each match one line at a time while also tracking key match day data.

- `getInput()` and `read()` handle various inputs for running the program.
- `addToMap()` and `printTop3()` are utility functions to handle some reptative tasks.
- `processMatch()` is where most of the logic lives, it is responsible for processing the current match and updating matchday data.
