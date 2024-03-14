# Azle REST API with ckBTC Integration
## Run Locally

Go to the project directory

```bash
  cd azle-api-rest-ckbtc
```

Install dependencies

```bash
  npm install
```

```bash
npm run btc:start
```

In another terminal run:

```bash
npm run icp:start
```

Open another terminal and run:

```bash
npm run icp:deploy:local
```

# How to mint ckBTC

Run the following command:

```bash
# Run three times this command, but wait 1 second between each exacution
npm run btc:mint --address=$ADDRESS
```

Wait for 5 seconds and make a request to `POST /users/:userId/balance`

Then, you can verify the user balance in this endpoint:

`GET /users/:userId/balance`
