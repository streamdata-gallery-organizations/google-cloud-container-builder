---
swagger: "2.0"
x-collection-name: Google Cloud Container Builder
x-complete: 0
info:
  title: Google Cloud Container Builder API Update Build Trigger
  description: |-
    Updates an BuildTrigger by its project ID and trigger ID.

    This API is experimental.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: cloudbuild.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/projects/{projectId}/builds:
    get:
      summary: Get Builds
      description: |-
        Lists previously requested builds.

        Previously requested builds may still be in-progress, or may have finished
        successfully or unsuccessfully.
      operationId: cloudbuild.projects.builds.list
      x-api-path-slug: v1projectsprojectidbuilds-get
      parameters:
      - in: query
        name: filter
        description: The raw filter text to constrain the results
      - in: query
        name: pageSize
        description: Number of results to return in the list
      - in: query
        name: pageToken
        description: Token to provide to skip to a particular spot in the list
      - in: path
        name: projectId
        description: ID of the project
      responses:
        200:
          description: OK
      tags:
      - Build
    post:
      summary: Starts Build
      description: |-
        Starts a build with the specified configuration.

        The long-running Operation returned by this method will include the ID of
        the build, which can be passed to GetBuild to determine its status (e.g.,
        success or failure).
      operationId: cloudbuild.projects.builds.create
      x-api-path-slug: v1projectsprojectidbuilds-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: ID of the project
      responses:
        200:
          description: OK
      tags:
      - Build
  /v1/projects/{projectId}/builds/{id}:
    get:
      summary: Get Build
      description: |-
        Returns information about a previously requested build.

        The Build that is returned includes its status (e.g., success or failure,
        or in-progress), and timing information.
      operationId: cloudbuild.projects.builds.get
      x-api-path-slug: v1projectsprojectidbuildsid-get
      parameters:
      - in: path
        name: id
        description: ID of the build
      - in: path
        name: projectId
        description: ID of the project
      responses:
        200:
          description: OK
      tags:
      - Build
  /v1/projects/{projectId}/builds/{id}:cancel:
    post:
      summary: Cancel Build
      description: Cancels a requested build in progress.
      operationId: cloudbuild.projects.builds.cancel
      x-api-path-slug: v1projectsprojectidbuildsidcancel-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of the build
      - in: path
        name: projectId
        description: ID of the project
      responses:
        200:
          description: OK
      tags:
      - Build
  /v1/projects/{projectId}/triggers:
    get:
      summary: Get Build Triggers
      description: |-
        Lists existing BuildTrigger.

        This API is experimental.
      operationId: cloudbuild.projects.triggers.list
      x-api-path-slug: v1projectsprojectidtriggers-get
      parameters:
      - in: path
        name: projectId
        description: ID of the project for which to list BuildTriggers
      responses:
        200:
          description: OK
      tags:
      - Trigger
    post:
      summary: Create Build Trigger
      description: |-
        Creates a new BuildTrigger.

        This API is experimental.
      operationId: cloudbuild.projects.triggers.create
      x-api-path-slug: v1projectsprojectidtriggers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: ID of the project for which to configure automatic builds
      responses:
        200:
          description: OK
      tags:
      - Trigger
  /v1/projects/{projectId}/triggers/{triggerId}:
    delete:
      summary: Delete Build Trigger
      description: |-
        Deletes an BuildTrigger by its project ID and trigger ID.

        This API is experimental.
      operationId: cloudbuild.projects.triggers.delete
      x-api-path-slug: v1projectsprojectidtriggerstriggerid-delete
      parameters:
      - in: path
        name: projectId
        description: ID of the project that owns the trigger
      - in: path
        name: triggerId
        description: ID of the BuildTrigger to delete
      responses:
        200:
          description: OK
      tags:
      - Trigger
    get:
      summary: Get Build Trigger
      description: |-
        Gets information about a BuildTrigger.

        This API is experimental.
      operationId: cloudbuild.projects.triggers.get
      x-api-path-slug: v1projectsprojectidtriggerstriggerid-get
      parameters:
      - in: path
        name: projectId
        description: ID of the project that owns the trigger
      - in: path
        name: triggerId
        description: ID of the BuildTrigger to get
      responses:
        200:
          description: OK
      tags:
      - Trigger
    patch:
      summary: Update Build Trigger
      description: |-
        Updates an BuildTrigger by its project ID and trigger ID.

        This API is experimental.
      operationId: cloudbuild.projects.triggers.patch
      x-api-path-slug: v1projectsprojectidtriggerstriggerid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: ID of the project that owns the trigger
      - in: path
        name: triggerId
        description: ID of the BuildTrigger to update
      responses:
        200:
          description: OK
      tags:
      - Trigger
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