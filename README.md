# cypher_app

## How to run 

1. Build image
   
    `docker build -t cipher-app .`

2. Run container

    `docker run -d -p 5000:5000 cipher-app`

4. Do a request
   
`
     curl --location 'http://127.0.0.1:5000/cipher' \
--header 'Content-Type: application/json' \
--data '{
    "message":"message to cypher",
    "key":"secret-key"
}' 
`
