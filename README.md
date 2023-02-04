# ring-client-example

This is an example project that uses the `ring-client-api` npm package to access the Ring API from Node.js. It is intended to show a basic project structure with proper TypeScript configuration.

## Setup

- (Optional) Fork this repository if you want to push changes to your own copy
- Clone the repository to your local environment
- Run `npm i` (assuming you already have [Node.js](https://nodejs.org/) installed)

## Authentication

- Run `npm run auth` to start the process. It should prompt you for email/password/token
- You will see a refresh token output like `"refreshToken": "eyJhbGciOi...afa1"`. You need to extract the value from the second part of this output, between the double quotes.
- Create a `.env` file in the root directory of this project and insert the following contents, replacing value with the one you got from the auth command above. _Make sure you don't include the quotes_:

```text
RING_REFRESH_TOKEN=eyJhbGciOi...afa1
```

## Run the Example

The example can be found in the [example.ts](./example.ts) file. Once you have followed the Authentication steps, you can start it by running `npm start`

## Additional Examples

Additional examples of how to use the `ring-client-api` can be found in <https://github.com/dgreif/ring/tree/main/packages/examples>
