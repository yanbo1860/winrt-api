---
-api-id: M:Windows.Gaming.Input.FlightStick.FromGameController(Windows.Gaming.Input.IGameController)
-api-type: winrt method
---

<!-- Method syntax.
public FlightStick FlightStick.FromGameController(IGameController gameController)
-->

# Windows.Gaming.Input.FlightStick.FromGameController

## -description

Returns the given game controller as a flight stick.

## -params

## -param gameController

The game controller to be returned as a flight stick.

## -returns

The flight stick that was returned from the given game controller.

## -remarks

## -see-also

* [Windows.Gaming.Input.IGameController](igamecontroller.md)

## -examples

<!--In the following example, the app gets the first available [RawGameController](rawgamecontroller.md) object, and tries to access this game controller via the `FlightStick` class.

```csharp
FlightStick flightStick = null;

if (RawGameController.RawGameControllers.Count > 0)
{
    RawGameController rawGameController = RawGameController.RawGameControllers[0];
    flightStick = FlightStick.FromGameController(rawGameController);
}

if (flightStick != null) 
{
    // Assign a standard button mapping to this controller.
}
```-->