swagger: "2.0"
x-collection-name: Auth0
x-complete: 1
info:
  title: Auth0 Users API
  version: v1
host: login.auth0.com
basePath: /users
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /blacklists/tokens:
    get:
      summary: Get Blacklists Tokens
      description: Get blacklists tokens.
      operationId: getBlacklistsTokens
      x-api-path-slug: blackliststokens-get
      parameters:
      - in: query
        name: aud
        description: The JWTs aud claim
      responses:
        200:
          description: OK
      tags:
      - Blacklists
      - Tokens
    post:
      summary: Post Blacklists Tokens
      description: Post blacklists tokens.
      operationId: postBlacklistsTokens
      x-api-path-slug: blackliststokens-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blacklists
      - Tokens
  /api/v2/blacklists/tokens:
    get:
      summary: Get Blacklists Tokens
      description: Get blacklists tokens.
      operationId: get_tokens
      x-api-path-slug: apiv2blackliststokens-get
      parameters:
      - in: query
        name: aud
        description: The JWTs aud claim
      responses:
        200:
          description: OK
      tags:
      - Blacklists
      - Tokens
    post:
      summary: Post Blacklists Tokens
      description: Post blacklists tokens.
      operationId: post_tokens
      x-api-path-slug: apiv2blackliststokens-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blacklists
      - Tokens