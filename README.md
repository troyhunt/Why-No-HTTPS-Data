# Why No HTTPS? The Raw Data!
This is the raw data that drives the whynohttps.com website. It's ordered by domain name so it's easy to see what changes from revision to revision.

##Input Files
There are 4 files which make up the bulk of the input:

1. http-sites.json : Sites that Scott Helme's crawler finds returning content over HTTP without redirecting to HTTPS with a 301 or 302
2. https-sites.json : Sites that Scott Helme's crawler finds explicitly redirecting from HTTP to HTTPS with a 301 or 302
3. top-1m.csv : The Tranco Top 1M websites used to rank the previous 2 lists
4. transport_security_state_static.json : Sites on the HSTS preload list

Scott publishes all his data publicly at [crawler.ninja](https://crawler.ninja/files/json/).

##Output Files
There are 2 main classes of file:

1. countries.json : A list of countries for which data has been prepared
2. top100.json : The 100 largest websites not redirecting HTTP to HTTPS
3. top50-[country code].json : The 50 largest websites for the given country not redirecting HTTP to HTTPS

##Notes
There's many reasons why a site might appear on this list that you *think* shouldn't be there. Read the launch blog post [Why No HTTPS? Here's the World's Largest Websites Not Redirecting Insecure Requests to HTTPS](https://www.troyhunt.com/why-no-https-heres-the-worlds-largest-websites-not-redirecting-insecure-requests/) and follow-up post [Why No HTTPS? Questions Answered, New Data, Path Forward](https://www.troyhunt.com/why-no-https-questions-answered-new-data-path-forward/) for more on that.

At present, the data is updated on an ad hoc basis.
