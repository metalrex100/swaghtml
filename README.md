# swaghtml

## Overview
Swaghtml generates html file with Swagger UI from swagger specification.

Supported swagger specification formats:
* json
* yaml 

## Getting started

Download swaghtml by using:
```sh
$ go get -u github.com/metalrex100/swaghtml
```

## Usage

Run:
```sh
swaghtml gen
```
 
By default swaghtml will search file with name **swagger.json** in your current directory and will output data to file with name **swagger.html**.

You can specify paths to input and output files with `--input (-i)` and `--output (-o)` flags:
```sh
swaghtml gen -i path_to_input_file -o path_to_output_file
```

## swaghtml cli
```sh
$ swaghtml gen -h
Generate html file from json/yaml spec.

Usage:
  swaghtml gen [flags]

Flags:
  -h, --help            help for gen
  -i, --input string    Path to input file with swagger spec. Can be json or yaml. (default "swagger.json")
  -o, --output string   Path to output html file. (default "swagger.html")
```