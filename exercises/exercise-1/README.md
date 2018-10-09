# Exercise 1: Writing your First API Specification

In this exercise, you will

Introduction

- Build NodeConf App (explain it)
- 2 different teams, one backend & one frontend (us)
- Need to establish an API.
- Writing our first API
- Lets identify objects (Speakers, Workshops, etc)

Input: Describe a final product that we’ll be looking to build
Identify functionality
Analyze resources and methods that we’ll need

Output: OAS Document (API Spec)
Download and Import in Postman Collection
Push directly to Github

## Use SwaggerHub to create an OAS document

SwaggerHub is TBD.

### Create your first OAS document in SwaggerHub

1. Open a new browser tab and navigate to the Swagger's Online Editor, [SwaggerHub](https://app.swaggerhub.com/).
1. Create a new account associated with your GitHub profile or log in to your account.

![Sign in to SwaggerHub]()

1. In the left panel, click the **Create New** button and select **Create new API**.

![Create new API]()

1. In the **Select a Template or create a Blank API** popup, enter the following info and then click **Create API**.

   - OpenAPI version: `2.0`
   - Template: `-- None --`
   - Name: `nodeconf-api`
   - Version: `1.0.0`
   - Title: `NodeConf API`
   - Description: `This is the API for the NodeConf`
   - Visibility: `Private`
   - Auto Mock API: `ON`
   - Owner: <your-user>.

   ![Create API modal info]()

   > **Note:** Why Swagger 2.0

After the API is created, you will be redirected to your new OAS document. Some information will be filled in for you, like the swagger version, the information of the API (version, title and description), an empty paths field and some other stuff autogenerated by the Auto Mocking Plugin (we'll see what this is later in the exercise).

![Your first OAS document in SwaggerHub]()

### Implement your first OAS document

Now it's time to implement our first document using the OAS/Swagger specification. We need to:

- Retrieve the list of Speakers of an specific conference.
- Retrieve the list of Activities of an specific conference, that may have one or more Speakers.
- Retrieve the Agenda of the current conference, composed by one or more activities.
- Finally, add the ability to provide feedback to the Activities.

Let's start

1. Write basic spec.
1. Use right panel - Spec read & Mocking Service - Try it out! functionality.

## Leverage Swagger capabilities to improve your OAS document

1. Reuse parameters by redefining a type (editionId)
1. Improve query by using an enum (event types). Explain that swagger 3.0 has a better way.
1. Define default response with ErrorResponse object

## Test your newly created API

1. Download Postman Collection and start hitting the API (mocking service)

## Bonus track

1. Add POST, PATCH and PUT (here).
1. Push OAS document (API spec) in GitHub’s backend repo.