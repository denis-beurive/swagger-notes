# Swagger editor

The installation procedure you can find on the official Swagger web-site ([here](https://swagger.io/docs/open-source-tools/swagger-editor/) or [here](https://github.com/swagger-api/swagger-editor)) is not  good.

Below, a procedure that works...

* Install [NodeJS](https://nodejs.org/en/download)
* Install the NodeJs module `http-server`: `npm install -g http-server`
* Install Swagger Editor: `npm i swagger-editor-dist`

Move to the directory where the module `swagger-editor-dist` has been installed. Under Windows, it should be `"%HOMEDRIVE%%HOMEPATH%\node_modules"`.

Make sure that the module `swagger-editor-dist` is installed under the directory `"%HOMEDRIVE%%HOMEPATH%\node_modules"`.

```dosbatch
DIR "%HOMEDRIVE%%HOMEPATH%\node_modules"
...
30/03/2023  17:25    <DIR>          swagger-editor-dist
...
```

Then start the HTTP server:

```dosbatch
CD "%HOMEDRIVE%%HOMEPATH%\node_modules"
http-server swagger-editor-dist
...
Available on:
  http://192.168.1.100:8080
  http://192.168.150.1:8080
  http://192.168.159.1:8080
  http://127.0.0.1:8080
Hit CTRL-C to stop the server
```

Now, you can open one of the URLs listed above in your browser.

