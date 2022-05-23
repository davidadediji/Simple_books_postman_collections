# Simple_books_postman_collections

# Postman- Newman with jenkins

Install newman with 

```bash
npm install -g newman
```

to install html-extra

```bash
npm install -g newman-reporter-htmlextra
```

1. To run newman on your single API collection
    1. go to api public collection to get the url for obtaining the single collection url on postman
    2. generate an API key from your account.
    3. replace {{collection_id}} with the actual collection id and add api-key as a parameter
    4. Get the JSON schema obtained and try 
        
        ```bash
        newman run <schema>
        ```
        

1. To get reports 

```bash
newman run <shema url> --reporters cli,htmlextra
```

1. Jenkins
    1. create a new item in jenkins
