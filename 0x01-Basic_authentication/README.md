## Basic authentication

The HTTP Authorization request header can be used to provide credentials that authenticate a user agent with a server, allowing access to a protected resource.

The Authorization header is usually, but not always, sent after the user agent first attempts to request a protected resource without credentials. The server responds with a 401 Unauthorized message that includes at least one WWW-Authenticate header. This header indicates what authentication schemes can be used to access the resource (and any additional information needed by the client to use them). The user-agent should select the most secure authentication scheme that it supports from those offered, prompt the user for their credentials, and then re-request the resource (including the encoded credentials in the Authorization header).
