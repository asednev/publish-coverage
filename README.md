# publish-coverage

```
Usage 
$ publish-coverage <input>

Options
  --index, -ix         Index name in elastic search (e.g. coverage_stats-YYYY.MM)
                       YYYY, MM will be replaced with actual date
  --file, -f           Path to coverage-summary.json
  --elasticUrl, -url   Elastic Search url (default http://localhost:9200)
  --debug, -r          Output debug information
  --appName            Name of the application, added to metrics
  --appVersion         Version of the application, added to metrics
  --package            Path to package.json to read application name and version from
                       (takes precedence over --appName & --appVersion)

Examples

$ publish-coverage \
    --index="coverage-YYYY.MM" \
    --file="coverage/report-html/coverage-summary.json" \
    --package="./package.json"
```