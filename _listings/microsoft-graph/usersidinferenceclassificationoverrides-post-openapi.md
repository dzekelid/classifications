---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Create Inference Classification Override
  description: Create inferenceClassificationOverride Create an override for a sender
    identified by an SMTP address. Future messages from that SMTP address will be
    consistently classified as specified in the override.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/inferenceClassification/overrides:
    post:
      summary: Create Inference Classification Override
      description: Create inferenceClassificationOverride Create an override for a
        sender identified by an SMTP address. Future messages from that SMTP address
        will be consistently classified as specified in the override.
      operationId: CreateInferenceClassificationOverride
      x-api-path-slug: meinferenceclassificationoverrides-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      responses:
        200:
          description: OK
      tags:
      - Inference
      - Classification
      - Override
  /users/{id}/inferenceClassification/overrides:
    post:
      summary: Create Inference Classification Override
      description: Create inferenceClassificationOverride Create an override for a
        sender identified by an SMTP address. Future messages from that SMTP address
        will be consistently classified as specified in the override.
      operationId: CreateInferenceClassificationOverride
      x-api-path-slug: usersidinferenceclassificationoverrides-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Inference
      - Classification
      - Override
  /me/inferenceClassification/overrides/{id}:
    delete:
      summary: Delete Inference Classification Override
      description: Delete inferenceClassificationOverride Delete an override specified
        by its ID.
      operationId: DeleteInferenceClassificationOverride
      x-api-path-slug: meinferenceclassificationoverridesid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Inference
      - Classification
      - Override
  /users/{id}/inferenceClassification/overrides/{id}:
    delete:
      summary: Delete Inference Classification Override
      description: Delete inferenceClassificationOverride Delete an override specified
        by its ID.
      operationId: DeleteInferenceClassificationOverride
      x-api-path-slug: usersidinferenceclassificationoverridesid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Inference
      - Classification
      - Override
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