# Yarp.Basic.Template
Project Template to quickly setup a basic reverse proxy using YARP. This template generates a simple .Net6 web app with the default options as found in the [YARP Getting Started](https://microsoft.github.io/reverse-proxy/articles/getting-started.html#net-6-support) documentation page.

## Usage:

Use this template by running `dotnet new yarp-basic`. There is only one required argument: `-f` which is the URL where the requests will be proxied to. You can also run `dotnet run yarp-basic -h` for more command line arguments. After that you can run `dotnet run` to run the proxy.

Example: `dotnet new yarp-basic -f https://httpbin.org`

## Running locally:

To install the template locally, you can run `dotnet new -i templates/yarp-basic/`

After any changes to the template you need to reinstall the package and clear the cache by running:

`dotnet new -u templates\yarp-basic && dotnet new -i templates\yarp-basic && dotnet new --debug:rebuildcache`