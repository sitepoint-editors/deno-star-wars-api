# How to Fetch Data From a 3rd Party API in Deno

A simple CLI tool which allows a user to query the [StarWars API](https://swapi.dev/), specifying a resource (film, person, or planet) and a search term.

## Requirements

* [Deno](https://deno.land/#installation)

## Installation Steps

1. Clone repo
2. Query the API like so: `deno run --allow-net=swapi.dev index.ts --resource=["films"|"people"|"planets"] --query="search term"`

### Example Usage:

```
$ deno run --allow-net=swapi.dev index.ts --resource films --query phantom
1 result
The Phantom Menace
=> Directed by George Lucas
=> Released on 1999-05-19

$ deno run --allow-net=swapi.dev index.ts --resource people --query jar jar
1 result
Jar Jar Binks
=> Height: 196
=> Mass:   66

$ deno run --allow-net index.ts --resource planets --query alderaan
1 result
Alderaan
=> Terrain:      grasslands, mountains
=> Population:   2000000000
```

## License

SitePoint's code archives and code examples are licensed under the MIT license.

Copyright © 2021 SitePoint

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
