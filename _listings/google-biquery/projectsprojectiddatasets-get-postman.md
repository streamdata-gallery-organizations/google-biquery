{
  "info": {
    "name": "Google BigQuery API Get Datasets",
    "_postman_id": "691d6cfa-78ff-4822-bdc8-8aaff4249e55",
    "description": "Lists all datasets in the specified project to which you have been granted the READER dataset role.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "dataset",
      "item": [
        {
          "id": "c45d66f4-1d9e-4421-a4de-c57e1b40ef17",
          "name": "bigquery.datasets.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "bigquery",
                "v2",
                "projects/:projectId/datasets"
              ],
              "query": [
                {
                  "key": "all",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "maxResults",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all datasets in the specified project to which you have been granted the READER dataset role"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "370dd4ef-de94-4f50-9da0-58f40e3ef64b"
            }
          ]
        }
      ]
    }
  ]
}