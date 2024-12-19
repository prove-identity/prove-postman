# Prove Postman Collections

Welcome to the Postman Collections Guide for Prove API! If you're looking to get started with the Prove API quickly without writing additional code, this is the perfect place to begin.

[<img src="https://run.pstmn.io/button.svg" alt="Run In Postman" style="width: 128px; height: 32px;">](https://god.gw.postman.com/run-collection/38260294-894dfff1-97ba-4f75-bd7f-ecaad30fcd18?action=collection%2Ffork&source=rip_markdown&collection-url=entityId%3D38260294-894dfff1-97ba-4f75-bd7f-ecaad30fcd18%26entityType%3Dcollection%26workspaceId%3D2b2087c9-2e13-49f6-b76f-797abbe1b52c#?env%5BProve%20Sandbox%20Pre-Fill%20with%20Milo%20Pinson%5D=W3sia2V5IjoiY29ycmVsYXRpb25JZCIsInZhbHVlIjoiIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6ImFueSIsInNlc3Npb25WYWx1ZSI6IiIsImNvbXBsZXRlU2Vzc2lvblZhbHVlIjoiIiwic2Vzc2lvbkluZGV4IjowfSx7ImtleSI6ImZpcnN0TmFtZSIsInZhbHVlIjoiTWlsbyIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJkZWZhdWx0Iiwic2Vzc2lvblZhbHVlIjoiTWlsbyIsImNvbXBsZXRlU2Vzc2lvblZhbHVlIjoiTWlsbyIsInNlc3Npb25JbmRleCI6MX0seyJrZXkiOiJsYXN0TmFtZSIsInZhbHVlIjoiUGluc29uIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6ImRlZmF1bHQiLCJzZXNzaW9uVmFsdWUiOiJQaW5zb24iLCJjb21wbGV0ZVNlc3Npb25WYWx1ZSI6IlBpbnNvbiIsInNlc3Npb25JbmRleCI6Mn0seyJrZXkiOiJkb2IiLCJ2YWx1ZSI6IjE5ODEtMDEtMTciLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6IjE5ODEtMDEtMTciLCJjb21wbGV0ZVNlc3Npb25WYWx1ZSI6IjE5ODEtMDEtMTciLCJzZXNzaW9uSW5kZXgiOjN9LHsia2V5Ijoic3NuIiwidmFsdWUiOiI4NDczNTA1OTYiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6Ijg0NzM1MDU5NiIsImNvbXBsZXRlU2Vzc2lvblZhbHVlIjoiODQ3MzUwNTk2Iiwic2Vzc2lvbkluZGV4Ijo0fSx7ImtleSI6ImFkZHJlc3MiLCJ2YWx1ZSI6IjYzNzcgQmlyY2h3b29kIEhpbGwiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6IjYzNzcgQmlyY2h3b29kIEhpbGwiLCJjb21wbGV0ZVNlc3Npb25WYWx1ZSI6IjYzNzcgQmlyY2h3b29kIEhpbGwiLCJzZXNzaW9uSW5kZXgiOjV9LHsia2V5IjoiY2l0eSIsInZhbHVlIjoiTGl0dGxldG9uIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6ImRlZmF1bHQiLCJzZXNzaW9uVmFsdWUiOiJMaXR0bGV0b24iLCJjb21wbGV0ZVNlc3Npb25WYWx1ZSI6IkxpdHRsZXRvbiIsInNlc3Npb25JbmRleCI6Nn0seyJrZXkiOiJwb3N0YWxDb2RlIiwidmFsdWUiOiI4MDE2MS0yMDAxIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6ImRlZmF1bHQiLCJzZXNzaW9uVmFsdWUiOiI4MDE2MS0yMDAxIiwiY29tcGxldGVTZXNzaW9uVmFsdWUiOiI4MDE2MS0yMDAxIiwic2Vzc2lvbkluZGV4Ijo3fSx7ImtleSI6InJlZ2lvbiIsInZhbHVlIjoiQ08iLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6IkNPIiwiY29tcGxldGVTZXNzaW9uVmFsdWUiOiJDTyIsInNlc3Npb25JbmRleCI6OH0seyJrZXkiOiJlbWFpbEFkZHJlc3MiLCJ2YWx1ZSI6Im1waW5zb25tQGR5bmRucy5vcmciLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6Im1waW5zb25tQGR5bmRucy5vcmciLCJjb21wbGV0ZVNlc3Npb25WYWx1ZSI6Im1waW5zb25tQGR5bmRucy5vcmciLCJzZXNzaW9uSW5kZXgiOjl9LHsia2V5IjoicGhvbmVOdW1iZXIiLCJ2YWx1ZSI6IjIwMDEwMDE2OTUiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6IjIwMDEwMDE2OTUiLCJjb21wbGV0ZVNlc3Npb25WYWx1ZSI6IjIwMDEwMDE2OTUiLCJzZXNzaW9uSW5kZXgiOjEwfSx7ImtleSI6ImlwQWRkcmVzcyIsInZhbHVlIjoiIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6ImRlZmF1bHQiLCJzZXNzaW9uVmFsdWUiOiIiLCJjb21wbGV0ZVNlc3Npb25WYWx1ZSI6IiIsInNlc3Npb25JbmRleCI6MTF9LHsia2V5IjoiZmxvd1R5cGUiLCJ2YWx1ZSI6Im1vYmlsZSIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJkZWZhdWx0Iiwic2Vzc2lvblZhbHVlIjoibW9iaWxlIiwiY29tcGxldGVTZXNzaW9uVmFsdWUiOiJtb2JpbGUiLCJzZXNzaW9uSW5kZXgiOjEyfSx7ImtleSI6ImZpbmFsVGFyZ2V0VXJsIiwidmFsdWUiOiJodHRwczovL3Byb3ZlLmNvbSIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJkZWZhdWx0Iiwic2Vzc2lvblZhbHVlIjoiaHR0cHM6Ly9wcm92ZS5jb20iLCJjb21wbGV0ZVNlc3Npb25WYWx1ZSI6Imh0dHBzOi8vcHJvdmUuY29tIiwic2Vzc2lvbkluZGV4IjoxM30seyJrZXkiOiJzbXNNZXNzYWdlIiwidmFsdWUiOiJDdXN0b21pemFibGUgc21zIG1lc3NhZ2UuIENvZGU6ICMjIyMiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6IkN1c3RvbWl6YWJsZSBzbXMgbWVzc2FnZS4gQ29kZTogIyMjIyIsImNvbXBsZXRlU2Vzc2lvblZhbHVlIjoiQ3VzdG9taXphYmxlIHNtcyBtZXNzYWdlLiBDb2RlOiAjIyMjIiwic2Vzc2lvbkluZGV4IjoxNH1d)

For more detailed information about the Prove API, visit [the Prove Developer Documentation](https://developer.prove.com/).

Don't feel like reading? Check out our [full API documentation](https://developer.prove.com/docs).

## Table of contents

- [Getting started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Configuration](#configuration)
- [Making API calls](#making-api-calls)
  - [Authentication](#authentication)
  - [Pre-Fill Flow](#pre-fill-flow)
- [Test Users](#test-users)
- [Get credentials](#get-credentials)
- [Environment Variables](#environment-variables)

## Getting started

Follow these steps to quickly get started with the [Prove API](https://developer.prove.com/):

1. [Sign up](https://portal.prove.com/en/signup) with Prove to get your API credentials
2. Fork the collection from [Prove's public workspace](https://www.postman.com/prove-eng/prove-link-api-testing/collection/93r30p4/prove-api?action=share&source=collection_link&creator=38260294) in Postman
3. Set up your environment variables as described in the [Configuration](#configuration) section

### Prerequisites

Before you begin, make sure you have:

- [Postman](https://www.getpostman.com/downloads/) installed
- A [Prove Account](https://portal.prove.com/en/signup)

### Configuration

The Prove Postman collection uses [Postman environment variables](https://learning.postman.com/docs/sending-requests/variables/) to simplify API requests. To set up your environment:

1. Fork the environment template from the Prove Developers Workspace
2. Create a new environment in Postman
3. Set the following environment variables:
   - `API_BASE_URL`: https://platform.uat.proveapis.com
   - `CLIENT_ID`: Your Prove client ID
   - `CLIENT_SECRET`: Your Prove client secret

To get your API credentials:

1. Log in to the [Portal](https://portal.prove.com/en/login)
2. Navigate to the **Pre-Fill** section
3. Create a new project
4. Access your project settings to view credentials

## Making API calls

### Authentication

The collection uses OAuth 2.0 for authentication:

1. The collection automatically handles token generation using your credentials
2. Tokens are obtained using the `/token` endpoint
3. All subsequent requests will include the authentication token

### Pre-Fill Flow

The Pre-Fill flow consists of the following endpoints that should be called in order:

1. `/v3/start` - Initiates the Pre-Fill flow
2. `/v3/validate` - Validates the initiated flow
3. `/v3/challenge` - Handles the challenge step
4. `/v3/complete` - Completes the Pre-Fill process

Each endpoint will return `success: true` when called correctly in sequence.

## Get credentials

To obtain your sandbox credentials:

1. Log in to the [Prove Portal](https://portal.prove.com/en/login)
2. Navigate to the **Pre-Fill** page from the left-side navigation
3. Create a new project by clicking **New Project**
4. Click on your project name
5. Access Settings > Credentials tab to view your API credentials

## Test Users

The collection comes pre-configured with test data for "Milo Pinson" for sandbox testing. For additional test users and scenarios, refer to the [Sandbox testing documentation](https://developer.prove.com/docs/prove-pre-fill-sandbox-testing#prove-pre-fill-test-users).

## Manual testing

The postman collection allows you to run through the Pre-Fill flow in this order:

- `/v3/start`
- `/v3/validate`
- `/v3/challenge`
- `/v3/complete`

You should be able to receive a `success=true` in the response bodies for each of the endpoints if you call them in order.

## Environment Variables

The following environment variables are used in the collection:

- Core Configuration:
  - `API_BASE_URL`
  - `CLIENT_ID`
  - `CLIENT_SECRET`

- User Information:
  - `flowType`
  - `phoneNumber`
  - `finalTargetUrl`
  - `dob`
  - `emailAddress`
  - `ssn`
  - `smsMessage`
  - `ipAddress`
  - `firstName`
  - `lastName`
  - `address`
  - `city`
  - `region`
  - `postalCode`

Make sure to set these variables in your environment before making API calls.

## Support

If you have any questions or need assistance, please contact support@prove.com.

