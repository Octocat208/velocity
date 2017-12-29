[<- Back to the cncf/velocity README.md file](../README.md)

## Guide to the CNCF projects chart creation

`analysis.rb` can be used to create data for a Cloud Native Computing Foundation projects bubble chart such as this one
![sample chart](./linuxfoundation_chart_example.png?raw=true "CNCF projects")

The chart itself can be generated in a [google sheet](https://docs.google.com/spreadsheets/d/1_DIvQpaPRecRONWeTh5pp3WOgbGcsY4JOPMBisizJqg/)
or as a stand-alone [html page](../charts/LF_bubble_chart.html). Details on usage of google chart api are [here](https://developers.google.com/chart/interactive/docs/gallery/bubblechart).<br />The first option is a copy/paste of resulting data where the second presents more control to the look of the chart but data insertion is a little difficult.

#### Chart data
Go to this [CNCF page](https://www.linuxfoundation.org/projects/) to find a list of current projects.
For every project find a github repo and add it to a query such as [this one](../BigQuery/query_lf_projects_201611_201710.sql) appropriately - either as an org or a single repo. If a project does not have a GitHub repo or only lists a mirror, skip it for now but later add manually.
Run the query on https://bigquery.cloud.google.com/queries/



