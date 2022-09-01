# Yarp.Basic.Template
Project Template to quickly setup a basic reverse proxy using YARP. This template generates a simple .Net6 web app with the default options as found in the [YARP Getting Started](https://microsoft.github.io/reverse-proxy/articles/getting-started.html#net-6-support) documentation page.

## Installation:

`dotnet new -i Ajdvoynos.Template.YARP-Basic`

## Usage:

`dotnet new yarp-basic -f https://yourUrlHere`. 

The only required argument is `-f` which is the URL where the requests will be proxied to. You can also run `dotnet run yarp-basic -h` for more command line arguments.

## Installation without npm:

Download the repository and run `dotnet new -i templates/yarp-basic/`.

After any changes to the template you need to reinstall the package and clear the cache by running:

`dotnet new -u templates\yarp-basic && dotnet new -i templates\yarp-basic && dotnet new --debug:rebuildcache`

## Publishing

To publish the package, you need to run `dotnet pack`, this will generate a .nupkg file that you can publish to nuget.