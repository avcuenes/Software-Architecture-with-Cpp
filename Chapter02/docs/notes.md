# Architectural Styles

## Deciding between stateful and stateless approaches

As the name suggests, stateful software's behavior depends on its internal state.

If the service was stateless, however, then each request coming to it would need to
contain all the data needed to process it successfully. This means that the requests
would get bigger and use up more bandwidth, but on the other hand, it would
allow for better performance and scaling of the service.

## Stateless and stateful services

A stateless system doesn’t store information about past interactions with the system. Therefore, each interaction with the system is like the first interaction with it.

A stateful system remembers previous interactions with the system and stores information about them. As a result, new interactions with the system may produce different outputs than previous interactions.

Statelessness is fundamental in modern internet services. The HTTP protocol is
stateless, while many service APIs, for example, Twitter's, are stateless as well.
REST, which Twitter's API relies on, is designed to be functionally stateless. The
whole concept behind this acronym, Representational State Transfer (REST),
carries the notion that all the state required for processing the request must be
transferred within it. If this is not the case, you can't say you have a RESTful
service.
If you're building an online store, you probably want to store information
pertaining to your customers, such as their order history and shipping addresses.
The client on the customer's side probably stores an authentication cookie, while
the server will probably store some user data in a database. The cookie replaces
our need for managing a session, as it'd be done in a stateful service


## Understanding monoliths—why they should be avoided and recognizing exceptions
The simplest architectural style in which you can develop your application is a
monolithic one. This is why many projects are started using this style.


## References
1.<https://www.baeldung.com/cs/stateful-stateless-system>