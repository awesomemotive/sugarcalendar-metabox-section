# Sugar Calendar Metabox Section Example

A simple example of how to create a metabox section.

This includes:

* Adding the section
* Registering meta keys, specifically for sanitization callbacks
* Combining meta keys into the Event array to be automatically saved
* Getting familiar with the `get/update/delete_event_meta()` functions

_All_ of your custom Event meta _needs to be_ registered, and you do not need to sanitize your posted values, nor do you need to do your own Nonce checks.

If you need to save meta data to the host Post (instead of the Event itself) you can use `$event->object_id` instead of `$event->id`. If you are unsure, you should probably stick to storing your meta with the Event (and not the Post) to ensure everything is primed and ready in the right areas.
