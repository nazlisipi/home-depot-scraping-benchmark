# Home Depot Scraping Benchmark

AIMultiple benchmark of five web data providers (Apify, Nimble, Oxylabs, SerpApi and Zyte) on Home Depot product and search pages. The study measures success rate and end-to-end completion time.

> [Read the benchmark on AIMultiple](https://aimultiple.com/home-depot-scraping)

## Workload

The results are taken from AIMultiple's e-commerce scraping benchmark, which covered 100 e-commerce domains. Each provider fetched the same 50 Home Depot product and search pages at 5 concurrent requests, for a total of 250 requests. A request counted as successful when it returned valid data under that benchmark's content validation rules.

SerpApi used its dedicated Home Depot engines for search and product pages. The other four sent both page types to one general endpoint: the Oxylabs universal source, the Zyte API, the Nimble Web API and the Apify E-commerce Scraping Tool actor.

## Benchmark results

Success rate and average end-to-end completion time per provider on the 50 Home Depot pages:

| Provider | Success rate (%) | Completion time (s) |
| --- | ---: | ---: |
| SerpApi | 100 | 1.3 |
| Oxylabs | 90 | 42 |
| Zyte | 36 | 84 |
| Apify | 28 | 37 |
| Nimble | 0 | 102 |

SerpApi, the only tested provider with engines built for Home Depot, succeeded on every page and was also the fastest. The article averages Oxylabs over all requests and Apify over successful requests only, so those two times are not directly comparable.

## Scope

The figures cover one live, US-only site with 50 pages per provider, and each provider ran with its own endpoint and settings. A changelog entry dated August 7, 2026 records that these pooled results replaced an earlier Home Depot methodology.

## Ownership

The benchmark implementation was developed for AIMultiple and belongs to AIMultiple. This repository contains a documentation summary. Source code and benchmark datasets are not distributed here.
