The original nginx container has some problems syncing file between your host(OSX) and your vm (Virtualbox VM). The reason is the parameter sendfile parameter. This image uses the default nginx configuration, but switches the sendfile parameter off, so syncing will work propably.

This is just a small workaround for a bug of virtualbox: https://www.virtualbox.org/ticket/9069
