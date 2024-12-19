# Prove Postman Collections

Welcome to the Postman Collections Guide for Prove API! If you're looking to get started with the Prove API quickly without writing additional code, this is the perfect place to begin.

[<img src="https://run.pstmn.io/button.svg" alt="Run In Postman" style="width: 128px; height: 32px;">](https://god.gw.postman.com/run-collection/38260294-894dfff1-97ba-4f75-bd7f-ecaad30fcd18?action=collection%2Ffork&source=rip_markdown&collection-url=entityId%3D38260294-894dfff1-97ba-4f75-bd7f-ecaad30fcd18%26entityType%3Dcollection%26workspaceId%3D2b2087c9-2e13-49f6-b76f-797abbe1b52c)

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

