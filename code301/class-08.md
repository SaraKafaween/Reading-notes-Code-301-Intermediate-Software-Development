# API Design

## RESTful web API design

![pic](https://th.bing.com/th/id/R.375ca0d969dfe3f244756fc2734af875?rik=FnhRpER90To0ow&riu=http%3a%2f%2fmaxoffsky.com%2fword%2fwp-content%2fuploads%2f2012%2f11%2fRESTful-API-design-1014x457.jpg&ehk=3AZNNZq8%2fNYcNVG5yCWTmHLpxv1vD6NjdmJmFKWIYf8%3d&risl=&pid=ImgRaw&r=0)

## Organize the API design around resources

Focus on the business entities that the web API exposes. For example, in an e-commerce system, the primary entities might be customers and orders. Creating an order can be achieved by sending an HTTP POST request that contains the order information. The HTTP response indicates whether the order was placed successfully or not. When possible, resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource).

## Define API operations in terms of HTTP methods

The HTTP protocol defines a number of methods that assign semantic meaning to a request. The common HTTP methods used by most RESTful web APIs are:

+ GET retrieves a representation of the resource at the specified URI. The body of the response message contains the details of the requested resource.
+ POST creates a new resource at the specified URI. The body of the request message provides the details of the new resource. Note that POST can also be used to trigger operations that don't actually create resources.
+ PUT either creates or replaces the resource at the specified URI. The body of the request message specifies the resource to be created or updated.
+ PATCH performs a partial update of a resource. The request body specifies the set of changes to apply to the resource.
+ DELETE removes the resource at the specified URI.
