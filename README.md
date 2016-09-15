# Scrapy: Just another Python scraper

This is just a scraper I built for finding, downloading, and replacing external assets in open source projects. It might be useful if you're trying to deploy an open-source project on a local network (without Internet access).

I built this one specifically for use with [FreeCodeCamp](https://github.com/FreeCodeCamp/FreeCodeCamp), but it should be useful for similar projects as well.

## Usage

Make sure you have Python and `wget` installed.

Just copy this script into your "open-source" project, and run `scrapy.py scrape`. 

This will build the external assets list, which you can then download by running `./scrapy.py download`.

Lastly, running `./scrapy.py internalize` will switch the external urls for local ones. 

Make sure to move place the assets on the `external` folder to a publicly available location on your server. This, of course, depends on your server configuration.