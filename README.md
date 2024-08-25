# Watchdog

A small plugin that can be used to let a monitoring service know that the server is still alive.
I use it with [Kuma Uptime](https://uptime.kuma.pet/) but anything that supports a simple webhook call should work.

In the case of Kuma uptime the webhook that is configured in the URL looks like this: `https://foo.bar/api/push/some_token?status=up&msg=OK&ping=`, the plugin will add the server FPS at the end of the URL - which can be easily removed if needed.