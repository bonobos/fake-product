# Bonobos Api Reference

> The Bonobos API is organized around REST. Our API has predictable resource-oriented URLs, accepts form-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, and verbs.

## Resources
---

### Products

> This is an array representing the products collection. You can retrieve it to see the available products.
> | **Endpoints** |
> | -------------------|
> | *Get* **/products**|
>
>#### Products Array
>
> Array of product hashes 
> 
>```json
>[
>  {
>    "name": "",
>    "sku": "",
>    "id": "",
>    "url": "",
>    "description": "",
>    "options": [],
>    "images": [],
>    "properties": {
>      "Detailings": [],
>      "Fabric": [],
>      "Model Details": [],
>      "country_of_origin": [],
>      "Care": [ ]
>   },
>    "price": {},
>    "selected_options": {}
>  },
>  {
>    "name": "",
>    "sku": "",
>    "id": "",
>    "url": "",
>    "description": "",
>    "options": [],
>    "images": [],
>    "properties": {
>      "Detailings": [],
>      "Fabric": [],
>      "Model Details": [],
>      "country_of_origin": [],
>      "Care": [ ]
>    },
>    "price": {},
>    "selected_options": {}
>   }
>]
>```



---

### Product

> This is an object representing the a specific product in the collection. You can retrieve it to see the products details.
>
>| **Endpoints** |
>| ------------------- |
>| *Get* **/products/:id** |
>
> #### Product Object
>
> #### Attributes
> ##### name <*string*>
>
>>Product name
>
> ##### sku <*string*> 
>
>> Product's sku identifier used by merchants
>
> ##### id** <*string*> 
>
>> Product's id
>
> ##### url <*string*> 
>
>> Product's url
>
>##### description<*string*> 
>
>> Product's short descrtiption
>
>##### options<*array*> 
>
>> This represents an array of product options
>
>##### images<*array*> 
>
>> This represents an array of product images
>
>##### properties<*object*> 
>
>> This represents an object of products properties with the following attibutes *Detailings*,
*Fabric*, *Model Details*, *country_of_origin* and *Care*
> 
>##### price<*object*> 
>
>> This represents the product's price object 
>
>##### selected_options<*object*> 
>
>> This represents the current products selected options used to surface the correct variant
>
>```json
>{
>  "name": "Stretch Washed Chino Shorts",
>  "sku": "SHORT00064",
>  "id": "1",
>  "url": "/products/stretch-washed-chino-shorts?color=sea%20stacks",
>  "description": "Our most popular shorts with the most customization. Choose your inseam length, color, waist size and even fit option! Fast, free shipping.",
>  "options": [
>    {
>      "name": "color",
>      "presentation": "Color",
>      "short_presentation": "Color",
>      "values": [
>        {
>          "name": "grey",
>          "presentation": "Grey",
>          "url": "https://bonobos-prod-s3.imgix.net/products/232150/original/SHORT_CHINO-SHORT_27768-GY437-32-5_swatch.jpg?1643838344="
>        },
>        {
>          "name": "khaki",
>          "presentation": "Khaki",
>          "url": "https://bonobos-prod-s3.imgix.net/products/232176/original/SHORT_CHINO-SHORT_27768-KH087-32-5_swatch.jpg?1643838344="
>        },
>        {
>          "name": "navy",
>          "presentation": "Navy",
>          "url": "https://bonobos-prod-s3.imgix.net/products/232099/original/SHORT_CHINO-SHORT_27768-BL007-32-5_swatch.jpg?1643838344="
>        }
>      ]
>    },
>    {
>      "name": "short-fit",
>      "presentation": "Short Fit",
>      "short_presentation": "Fit",
>      "values": [
>        {
>          "name": "slim",
>          "presentation": "Slim"
>        },
>        {
>          "name": "standard",
>          "presentation": "Standard"
>        },
>        {
>          "name": "athletic",
>          "presentation": "Athletic"
>        }
>      ]
>    },
>    {
>      "name": "short-waist",
>      "presentation": "Short Waist",
>      "short_presentation": "Waist",
>      "values": [
>        {
>          "name": "28",
>          "presentation": "28"
>        },
>        {
>          "name": "29",
>          "presentation": "29"
>        },
>        {
>          "name": "30",
>          "presentation": "30"
>        }
>      ]
>    },
>    {
>      "name": "short-length",
>      "presentation": "Short Length",
>      "short_presentation": "Length",
>      "values": [
>        {
>          "name": "5 in",
>          "presentation": "5 In"
>        },
>        {
>          "name": "7 in",
>          "presentation": "7 In"
>        }
>      ]
>    }
>  ],
>  "images": [
>      "https://bonobos-prod-s3.imgix.net/products/217723/original/SHORT_CHINO-SHORT_27814-BOY73-32-9_1.jpg?1642751178=",
>      "https://bonobos-prod-s3.imgix.net/products/217724/original/SHORT_CHINO-SHORT_27814-BOY73-32-9_3_hover.jpg?1642751178="
>  ],
>  "properties": {
>    "Detailings": [
>      "The stretch version of our classic washed chino.",
>      "Signature curved waistband and contrast pocket liner.",
>      "Italian slide snap at center front closure.",
>      "Buttons at back pockets."
>    ],
>    "Fabric": [
>      "98% Cotton | 2% Lycra; Stretch Cotton Twill"
>    ],
>    "Model Details": [
>      "Model is 6'2\" with a 32\" waist, and is wearing a size 32\" in Standard Fit."
>    ],
>    "country_of_origin": [
>      "Imported"
>   ],
>    "Care": [
>      "Machine wash cold with like colors | Tumble dry low | Cool iron if needed | Do Not Bleach"
>    ]
>  },
>  "price": {
>    "price_numeric": 69,
>    "price": "$69",
>    "full_price": "$79",
>    "on_sale": true
>  },
>  "selected_options": {
>    "color": "grey"
>  }
>}
>```
