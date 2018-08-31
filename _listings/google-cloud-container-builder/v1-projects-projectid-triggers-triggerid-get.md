---
swagger: "2.0"
info:
  title: Google Cloud Container Builder
  description: Builds container images in the cloud.
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
  /v1/projects/{projectId}/triggers/{triggerId}:
    get:
      summary: Get Build Trigger
      description: Gets information about a BuildTrigger
      operationId: cloudbuild.projects.triggers.get
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
      - trigger
definitions:
  Build:
    properties:
      buildTriggerId:
        description: This is a default description.
        type: post
      createTime:
        description: This is a default description.
        type: post
      finishTime:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      images:
        description: This is a default description.
        type: post
      logUrl:
        description: This is a default description.
        type: post
      logsBucket:
        description: This is a default description.
        type: post
      projectId:
        description: This is a default description.
        type: post
      startTime:
        description: This is a default description.
        type: post
      status:
        description: This is a default description.
        type: post
  BuildOperationMetadata:
    properties: []
  BuildOptions:
    properties:
      requestedVerifyOption:
        description: This is a default description.
        type: post
      sourceProvenanceHash:
        description: This is a default description.
        type: post
  BuildStep:
    properties:
      args:
        description: This is a default description.
        type: post
      dir:
        description: This is a default description.
        type: post
      entrypoint:
        description: This is a default description.
        type: post
      env:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      waitFor:
        description: This is a default description.
        type: post
  BuildTrigger:
    properties:
      createTime:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      disabled:
        description: This is a default description.
        type: post
      filename:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      substitutions:
        description: This is a default description.
        type: post
  BuiltImage:
    properties:
      digest:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
  CancelBuildRequest:
    properties: []
  CancelOperationRequest:
    properties: []
  Empty:
    properties: []
  FileHashes:
    properties:
      fileHash:
        description: This is a default description.
        type: post
  Hash:
    properties:
      type:
        description: This is a default description.
        type: post
      value:
        description: This is a default description.
        type: post
  ListBuildTriggersResponse:
    properties:
      triggers:
        description: This is a default description.
        type: post
  ListBuildsResponse:
    properties:
      builds:
        description: This is a default description.
        type: post
      nextPageToken:
        description: This is a default description.
        type: post
  ListOperationsResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: post
      operations:
        description: This is a default description.
        type: post
  Operation:
    properties:
      done:
        description: This is a default description.
        type: post
      metadata:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      response:
        description: This is a default description.
        type: post
  RepoSource:
    properties:
      branchName:
        description: This is a default description.
        type: post
      commitSha:
        description: This is a default description.
        type: post
      projectId:
        description: This is a default description.
        type: post
      repoName:
        description: This is a default description.
        type: post
      tagName:
        description: This is a default description.
        type: post
  Results:
    properties:
      buildStepImages:
        description: This is a default description.
        type: post
      images:
        description: This is a default description.
        type: post
  Source:
    properties: []
  SourceProvenance:
    properties:
      fileHashes:
        description: This is a default description.
        type: post
  Status:
    properties:
      code:
        description: This is a default description.
        type: post
      details:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
  StorageSource:
    properties:
      bucket:
        description: This is a default description.
        type: post
      generation:
        description: This is a default description.
        type: post
      object:
        description: This is a default description.
        type: post
x-collection-name: Google Cloud Container Builder
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