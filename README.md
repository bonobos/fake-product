# fake-product

## Usage
- add items to the `db.json` file to expose a resource and its payload.
- resources are defined in the top level of the json object like: 
```
{
  "<resource1>": <payload>,
  "<resource2>": <payload>
}
```
- resource payload is capped at 10kb of data max to use the [my-json-server](https://my-json-server.typicode.com) service.
- the api is exposed at `https://my-json-server.typicode.com/bonobos/fake-product/`
  - the api supports all crud operations
  - sample reequest: 
      - GET collection of products `https://my-json-server.typicode.com/bonobos/fake-product/products`
      - GET product with `:id` of 1 `https://my-json-server.typicode.com/bonobos/fake-product/products/1`