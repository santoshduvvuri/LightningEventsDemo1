# LightningEventsDemo1
LightningEventsDemo1

Lightning component events also support both capture and bubble phases, but there are some framework specificities in terms of syntax and behavior.

By default, component events are handled in the bubble phase, and that’s what most developers use.

To handle the capture phase, add a phase="capture" attribute to your event handler, like so:
Note that you can declare two handlers for the same event if you wish to handle both phases (one for bubble and one for capture).

You can query the event’s current propagation phase by calling event.getPhase() in your event handling function. This function returns either capture or bubble

List of components to the current package:

Lightning App: 
	• ComponentEventPlayground
Lightning Component Event: 
	• cmpEvent
Lightning Components:
	• container
	• eventEmitter
	• owner
