# This is the simple app for presenting the AWS amplify

## Prequesties

1. AWS Account(FreeTier also works)
2. Node.JS
3. Be AWESOME

## Applicaiton Stack

1. CloudFormation
2. DynamoDB
3. Graphql
4. AppSync
5. React
6. s3
7. CloudFront
8. Route53(Optional)

# ✍️ Write with me

A real-time collaborative blog post editor built with GraphQL, React, React Markdown, & AWS AppSync.

> Try it out at [www.writewithme.dev](https://www.writewithme.dev/#/)

![](writewithme.gif)

### Base schema

Here's the base schema:

```graphql
type Post @model {
  id: ID!
  clientId: ID!
  markdown: String!
  title: String!
  createdAt: String
}
```

We have a `Post` type that has a few properties. The most important property is the markdown. This is where we are keeping up with the state of the post.

We also have a `clientId` to properly handle GraphQL subscriptions on the client.

## Launching the app

Deploy this fullstack app with a single click to the Amplify Console:

[![amplifybutton](https://oneclick.amplifyapp.com/button.svg)](https://console.aws.amazon.com/amplify/home#/deploy?repo=https://github.com/winhtaikaung/awsmm-write-with-me)

### Run locally with the Amplify CLI

1. Clone the repo

```sh
git clone https://github.com/winhtaikaung/awsmm-write-with-me.git
```

2. Change into the directory & install dependencies

```sh
cd awsmm-write-with-me

npm install
```

3. Initialize the Amplify backend

```sh
amplify init
```

4. Push the application into your account

```sh
amplify push
```
