{
  "info": {
    "name": "Google BigQuery API Delete Dataset",
    "_postman_id": "db09b785-59d1-4d42-b9a4-47c4be5f8a09",
    "description": "Deletes the dataset specified by the datasetId value. Before you can delete a dataset, you must delete all its tables, either manually or by specifying deleteContents. Immediately after deletion, you can create another dataset with the same name.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "dataset",
      "item": [
        {
          "id": "8eef6fc5-fb2f-45e6-9e23-ff8cee6a5c05",
          "name": "bigquery.datasets.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "bigquery",
                "v2",
                "projects/:projectId/datasets/:datasetId"
              ],
              "query": [
                {
                  "key": "deleteContents",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "datasetId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the dataset specified by the datasetId value"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce260813-9d23-4194-a5f8-3c6de40ab421"
            }
          ]
        }
      ]
    }
  ]
}