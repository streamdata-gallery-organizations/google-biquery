---
swagger: "2.0"
x-collection-name: Google Biquery
x-complete: 0
info:
  title: Google BigQuery API Get Datasets
  description: Lists all datasets in the specified project to which you have been
    granted the READER dataset role.
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /bigquery/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects:
    get:
      summary: Get Projects
      description: Lists all projects to which you have been granted any project role.
      operationId: bigquery.projects.list
      x-api-path-slug: projects-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Page token, returned by a previous call, to request the next
          page of results
      responses:
        200:
          description: OK
      tags:
      - Project
  /projects/{projectId}/datasets:
    get:
      summary: Get Datasets
      description: Lists all datasets in the specified project to which you have been
        granted the READER dataset role.
      operationId: bigquery.datasets.list
      x-api-path-slug: projectsprojectiddatasets-get
      parameters:
      - in: query
        name: all
        description: Whether to list all datasets, including hidden ones
      - in: query
        name: filter
        description: An expression for filtering the results of the request by label
      - in: query
        name: maxResults
        description: The maximum number of results to return
      - in: query
        name: pageToken
        description: Page token, returned by a previous call, to request the next
          page of results
      - in: path
        name: projectId
        description: Project ID of the datasets to be listed
      responses:
        200:
          description: OK
      tags:
      - Dataset
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---