# cypher_app

## How to run 

1. Build image
   
    `docker build -t cipher-app .`

2. Run container

    `docker run -d -p 5000:5000 cipher-app`

3. Do a request to ping

    `curl --location 'http://127.0.0.1:5000/ping'`

4. Do a request to cipher

    `curl --location 'http://127.0.0.1:5000/cipher' --header 'Content-Type: application/json' --data '{"message":"message to cipher","key":"secret-key"}'`

5. Do a request to decipher

    `curl --location 'http://127.0.0.1:5000/decipher' --header 'Content-Type: application/json' --data '{"message":"DD6D3DE855CA69F84CB685456829392491","key":"secret-key"}'`
