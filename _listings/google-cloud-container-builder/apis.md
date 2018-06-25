---
name: Google Cloud Container Builder
x-slug: google-cloud-container-builder
description: Google Cloud Container Builder lets you create Docker container images
  from application source code located in Google Cloud Storage. Container images created
  by Container Builder are automatically stored in Google Container Registry. You
  can deploy the container images you create on Google Container Engine, Google Compute
  Engine, Google App Engine flexible environment or other services where you can run
  applications from Docker containers.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/container-builder-lead.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Google Cloud Container Builder
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-container-builder/master/_listings/google-cloud-container-builder/apis.md
specificationVersion: "0.14"
apis:
- name: Google Cloud Container Builder API Get Builds
  x-api-slug: google-cloud-container-builder-api
  description: |-
    Lists previously requested builds.

    Previously requested builds may still be in-progress, or may have finished
    successfully or unsuccessfully.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/container-builder-lead.png
  humanURL: https://cloud.google.com/container-builder/
  baseURL: ://cloudbuild.googleapis.com////v1/projects/{projectId}/builds
  tags: Build
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-container-builder/master/_listings/google-cloud-container-builder/v1projectsprojectidbuilds-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-container-builder/master/_listings/google-cloud-container-builder/v1projectsprojectidbuilds-get-openapi.md
- name: Google Cloud Container Builder API Starts Build
  x-api-slug: google-cloud-container-builder-api
  description: |-
    Starts a build with the specified configuration.

    The long-running Operation returned by this method will include the ID of
    the build, which can be passed to GetBuild to determine its status (e.g.,
    success or failure).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/container-builder-lead.png
  humanURL: https://cloud.google.com/container-builder/
  baseURL: ://cloudbuild.googleapis.com////v1/projects/{projectId}/builds
  tags: Build
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-container-builder/master/_listings/google-cloud-container-builder/v1projectsprojectidbuilds-post-openapi.md
- name: Google Cloud Container Builder API Get Build
  x-api-slug: google-cloud-container-builder-api
  description: |-
    Returns information about a previously requested build.

    The Build that is returned includes its status (e.g., success or failure,
    or in-progress), and timing information.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/container-builder-lead.png
  humanURL: https://cloud.google.com/container-builder/
  baseURL: ://cloudbuild.googleapis.com////v1/projects/{projectId}/builds/{id}
  tags: Build
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-container-builder/master/_listings/google-cloud-container-builder/v1projectsprojectidbuildsid-get-openapi.md
- name: Google Cloud Container Builder API Cancel Build
  x-api-slug: google-cloud-container-builder-api
  description: Cancels a requested build in progress.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/container-builder-lead.png
  humanURL: https://cloud.google.com/container-builder/
  baseURL: ://cloudbuild.googleapis.com////v1/projects/{projectId}/builds/{id}:cancel
  tags: Build
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-container-builder/master/_listings/google-cloud-container-builder/v1projectsprojectidbuildsidcancel-post-openapi.md
- name: Google Cloud Container Builder API Get Build Triggers
  x-api-slug: google-cloud-container-builder-api
  description: |-
    Lists existing BuildTrigger.

    This API is experimental.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/container-builder-lead.png
  humanURL: https://cloud.google.com/container-builder/
  baseURL: ://cloudbuild.googleapis.com////v1/projects/{projectId}/triggers
  tags: Trigger
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-container-builder/master/_listings/google-cloud-container-builder/v1projectsprojectidtriggers-get-openapi.md
- name: Google Cloud Container Builder API Create Build Trigger
  x-api-slug: google-cloud-container-builder-api
  description: |-
    Creates a new BuildTrigger.

    This API is experimental.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/container-builder-lead.png
  humanURL: https://cloud.google.com/container-builder/
  baseURL: ://cloudbuild.googleapis.com////v1/projects/{projectId}/triggers
  tags: Trigger
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-container-builder/master/_listings/google-cloud-container-builder/v1projectsprojectidtriggers-post-openapi.md
- name: Google Cloud Container Builder API Delete Build Trigger
  x-api-slug: google-cloud-container-builder-api
  description: |-
    Deletes an BuildTrigger by its project ID and trigger ID.

    This API is experimental.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/container-builder-lead.png
  humanURL: https://cloud.google.com/container-builder/
  baseURL: ://cloudbuild.googleapis.com////v1/projects/{projectId}/triggers/{triggerId}
  tags: Trigger
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-container-builder/master/_listings/google-cloud-container-builder/v1projectsprojectidtriggerstriggerid-delete-openapi.md
- name: Google Cloud Container Builder API Get Build Trigger
  x-api-slug: google-cloud-container-builder-api
  description: |-
    Gets information about a BuildTrigger.

    This API is experimental.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/container-builder-lead.png
  humanURL: https://cloud.google.com/container-builder/
  baseURL: ://cloudbuild.googleapis.com////v1/projects/{projectId}/triggers/{triggerId}
  tags: Trigger
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-container-builder/master/_listings/google-cloud-container-builder/v1projectsprojectidtriggerstriggerid-get-openapi.md
- name: Google Cloud Container Builder API Update Build Trigger
  x-api-slug: google-cloud-container-builder-api
  description: |-
    Updates an BuildTrigger by its project ID and trigger ID.

    This API is experimental.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/container-builder-lead.png
  humanURL: https://cloud.google.com/container-builder/
  baseURL: ://cloudbuild.googleapis.com////v1/projects/{projectId}/triggers/{triggerId}
  tags: Trigger
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-container-builder/master/_listings/google-cloud-container-builder/v1projectsprojectidtriggerstriggerid-patch-openapi.md
- name: Google Cloud Container Builder API Get Operation State
  x-api-slug: google-cloud-container-builder-api
  description: |-
    Gets the latest state of a long-running operation.  Clients can use this
    method to poll the operation result at intervals as recommended by the API
    service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/container-builder-lead.png
  humanURL: https://cloud.google.com/container-builder/
  baseURL: ://cloudbuild.googleapis.com////v1/{name}
  tags: Operation
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-container-builder/master/_listings/google-cloud-container-builder/v1name-get-openapi.md
- name: Google Cloud Container Builder API Cancel Operation
  x-api-slug: google-cloud-container-builder-api
  description: |-
    Starts asynchronous cancellation on a long-running operation.  The server
    makes a best effort to cancel the operation, but success is not
    guaranteed.  If the server doesn't support this method, it returns
    `google.rpc.Code.UNIMPLEMENTED`.  Clients can use
    Operations.GetOperation or
    other methods to check whether the cancellation succeeded or whether the
    operation completed despite cancellation. On successful cancellation,
    the operation is not deleted; instead, it becomes an operation with
    an Operation.error value with a google.rpc.Status.code of 1,
    corresponding to `Code.CANCELLED`.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/container-builder-lead.png
  humanURL: https://cloud.google.com/container-builder/
  baseURL: ://cloudbuild.googleapis.com////v1/{name}:cancel
  tags: Operation
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-container-builder/master/_listings/google-cloud-container-builder/v1namecancel-post-openapi.md
- name: Google Cloud Container Builder API
  x-api-slug: google-cloud-container-builder-api
  description: Google Cloud Container Builder lets you create Docker container images
    from application source code located in Google Cloud Storage. Container images
    created by Container Builder are automatically stored in Google Container Registry.
    You can deploy the container images you create on Google Container Engine, Google
    Compute Engine, Google App Engine flexible environment or other services where
    you can run applications from Docker containers.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/container-builder-lead.png
  humanURL: https://cloud.google.com/container-builder/
  baseURL: ://cloudbuild.googleapis.com//
  tags: Google Cloud Container Builder
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-container-builder/master/_listings/google-cloud-container-builder/openapi.md
x-common:
- type: x-documentation
  url: https://cloud.google.com/container-builder/docs/
- type: x-pricing
  url: https://cloud.google.com/container-builder/pricing
- type: x-website
  url: https://cloud.google.com/container-builder/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---