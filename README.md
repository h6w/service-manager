# service-manager
Libraries for managing services in a cross-platform way using the OS's own service manager.

Occasionally one needs to detect and manipulate system services.  (Bearing in mind the security risks of doing so.)  However, each init system (on POSIX) and every other platform (Windows, etc.) have different ways to manage and report services.  Many languages, on the other hand, runs on many of these systems, so this code provides a way to abstract those processes so that the rest of your code is simpler.

This is a collection of code that should operate similarly across platforms to provide a way to:

 1. Detect if a service is enabled or disabled, running or stopped
 2. Where possible, and providing the proper security measures are in place, allow a service to be enabled, disabled, started, stopped, or restarted.
 3. Report errors from the service so that applications can respond and/or report back to the user
 
