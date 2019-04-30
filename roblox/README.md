# Roblox Module API

All functions will return
bool Success, variant error_or_data
unless otherwise specified. If Success is false, error_or_data will always be the error message.

##### function API.Setup(string Host, int PORT[, string Authentication])
Host should be the location of your server without any trailing slashes. EX: http://my.ip.or.domain
Port should be the port you specified in your server.
Authentication should only be specified if there is a password set in the server.

##### function API.IsConnected()
Returns true or false, if the WebSocket proxy is already connected to a WebSocket server.

##### function API.GetConnection()
Returns the url that the WebSocket proxy is already connected to, or false if it isn't connected.

##### function API.