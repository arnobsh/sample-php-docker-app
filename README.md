# Apache2 Setup With Docker

Simple Docker file to set up the apache2 server  to run Php

## Installation By `"docker"`

Use the following commands to set up the server

```
docker build -t sitename .
```

## Getting it running

To run apache in a background process, simply start the container using the following command:

```
docker run -p 8080:80 -d sitename 
```

-p 8080:80 publishes port 80 in the container to 8080 on the host machine.
-d detaches from the process, use docker ps and docker stop to … stop.

To run the server in the bash

```
docker run -i -t -p 8080:80 sitename /bin/bash
```

## Installation By `"docker-compose"`

For running by docker-compose simply run the following command


```
docker-compose run -it apache_server bash
```

It will automatically run the apache and insert into bash

After running the service you will go to the link http://localhost:80/ and find the PHP application

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Let me know if you have any questions regarding the setup or if you have faced any problem let me know by email arnobsh@gmail.com

## License
[MIT](https://choosealicense.com/licenses/mit/)