# tippecanoe-docker
TippeCanoe on DockerHub

## How to use this

You can run tippecanoe by using `docker run alexgleith/tippecanoe`.

To run an container with local data mounted, and process it, do something like this:

```
	docker run --rm -v $(shell pwd)/data:/data alexgleith/tippecanoe \
		tippecanoe -o /data/example_out.mbtiles \
			--force \
			-l example_out -n "An Example Dataset" /data/example_in.json
```

More documentation is available at the [MapBox/Tippecanoe GitHub site](https://github.com/mapbox/tippecanoe).
