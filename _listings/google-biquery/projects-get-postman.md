{
  "info": {
    "name": "Google BigQuery API Get Projects",
    "_postman_id": "7a16770d-c598-46c7-8922-d780f14eefee",
    "description": "Lists all projects to which you have been granted any project role.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Project",
      "item": [
        {
          "id": "e9030878-1001-4fdb-8033-dd2ec1a04129",
          "name": "bigquery.projects.list",
          "request": {
            "url": "http://www.googleapis.com/bigquery/v2/projects?maxResults=%7B%7D&pageToken=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all projects to which you have been granted any project role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df11c72e-6bce-405a-9be5-3fc4b97c1ae8"
            }
          ]
        }
      ]
    }
  ]
}