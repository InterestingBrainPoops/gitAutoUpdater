# gitAutoUpdater
Is essentially a way for you to create a webhook for your applications by running a webserver.
  
  
## Usage: 
Update the config.json to match your usecase.
The `port` argument should be the port you want the webserver to listen on.
The `path` argument should be the URL route you want listened on.
Then you update the `run.sh` file to the commands you want used.

## How it works:
Listens for a POST request on the specified path and on that it runs the bash script you have specified.
It doesn't use any of the info from the POST payload, so you have to configure on your end when the POST request needs to be made.

## Contributing
Ill take a look at the PR and if it makes sense, then ill add it.
Build using `go build` and testing is redundant in this case, so its not there.


## Dependencies
No external dependencies, look in the releases for the executable for your OS.
## License
MIT Licence C 2021
