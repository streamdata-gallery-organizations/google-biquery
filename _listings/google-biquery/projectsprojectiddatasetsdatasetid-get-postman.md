{
  "info": {
    "name": "Google BigQuery API Get Dataset",
    "_postman_id": "3ad9b742-a5df-412b-9ca8-8bda1e039dee",
    "description": "Returns the dataset specified by datasetID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "dataset",
      "item": [
        {
          "id": "5fabbb54-7c9d-4212-a165-65cb786fc594",
          "name": "bigquery.datasets.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "bigquery",
                "v2",
                "projects/:projectId/datasets/:datasetId"
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the dataset specified by datasetID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8100a143-1134-45eb-b4b1-aeccb2e030ea"
            }
          ]
        }
      ]
    }
  ]
}