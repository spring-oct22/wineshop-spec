# Wine shop

* Normalize the given dataset wines_SPA.csv

```mermaid
erDiagram

Wine {
    Integer id
    String name
    Integer year
    Float rating
    Integer num_reviews
    Float price
    Integer body
    Integer acidity
    Integer winery_id
    Integer type_id
    Integer region_id
}
Winery {
    Integer id
    String name
}
Region {
    Integer id
    String name
    String country
}
Type {
    Integer id
    String name
}


Winery ||--o{ Wine : makes
Region ||--o{ Wine : harvests
Type ||--o{ Wine : belongs
```

* Build a RESTful API around the model implementing entity lists and all CRUD operations implementing the attached [OpenAPI specification](api-docs.yaml).

    * `/api/wine/{id}`
    * `/api/winery/{id}`
    * `/api/region/{id}`
    * `/api/type/{id}`

* Create unit tests.

* Create functional tests.

* Implement basic authentication.


(Data attribution: [fedesoriano](https://www.kaggle.com/fedesoriano))
