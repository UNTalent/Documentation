# Open API documentation v.1.0.2

Our API is free with a fair use, at your own risk. Attribution is welcome, ideally with direct links to the job offers hosted on untalent.org.

## Jobs API endpoints

All the jobs, including home-based positions, are available on this endpoint:
```
https://untalent.org/api/v1/jobs
```

Remote (home-based) jobs only:
```
https://untalent.org/api/v1/homebased
```

### Filters

To add a filter, use query parameters, for instance `?locationSlugs=geneva&areaSlugs=human-resources`

All the filters can be combined. The separator `+` can be used for multiple tags in the same category. When there are multiple tags, at least one of them must be present (_OR_). When multiple categories are used, each category will have at least one matching tag in the results (_AND_). When a tag does not exist, it is ignored.


* `locationSlugs`: the location, for instance `Geneva`, `Kenya`, `New-York`, or `Kenya+New-York` 
* `areaSlugs`: the slug version of the work area, for instance `human-resources`, `innovation`
* `levelSlugs`: the level of the contract, for instance `mid`, `consulting`, `volunteer`, `senior`


### Pagination

You can navigate between pages by adding `?page=2` to the url
