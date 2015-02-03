# SmartThings Z-wave Motion Sensor with Refresh

This repo is two main components.  The first is a Z-wave motion device that is identical to the standard Z-wave motion sensor devicetype.  This device has been modified to include a "refresh" capability that clears any active motion off the sensor.  This is partitionally useful for hardware that gets stuck, or when the Hub misses an update. 

The second component is a SmartApp that actually initiates the refresh on a regular interval. This is very similar to the excellent Pollster application, but using the Refresh command instead of Poll command. 

When paired together, these two scripts can offer a unique capability to clear stuck sensors.  Sometimes this happens if the Hub is unavailable during an inactive trigger, or if the device is producing an unusual signal.  For example, when using contact sensors as pressure sensors, the device state may remain "active" even though the device is not. 


