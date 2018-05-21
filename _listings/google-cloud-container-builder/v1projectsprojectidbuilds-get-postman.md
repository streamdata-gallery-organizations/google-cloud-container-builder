{
  "info": {
    "name": "Google Cloud Container Builder API Get Builds",
    "_postman_id": "ee2ab2c0-3836-4fb0-bf38-0338c7496889",
    "description": "Lists previously requested builds.\n\nPreviously requested builds may still be in-progress, or may have finished\nsuccessfully or unsuccessfully.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Build",
      "item": [
        {
          "id": "78be8588-6743-4553-876c-9d4b4ab2fe1b",
          "name": "cloudbuild.projects.builds.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "cloudbuild.googleapis.com",
              "path": [
                "v1/projects/:projectId/builds"
              ],
              "query": [
                {
                  "key": "filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageSize",
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
            "description": "Lists previously requested builds.\n\nPreviously requested builds may still be in-progress, or may have finished\nsuccessfully or unsuccessfully."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "259505e7-7b43-4489-8f50-06b353833e96"
            }
          ]
        }
      ]
    }
  ]
}