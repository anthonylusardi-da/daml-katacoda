The ledger and the HTTP JSON API server are running, your application is deployed and all parties
allocated. Let's see if we can start the UI!

```
cd create-daml-app
cd ui
export REACT_APP_LEDGER_ID=test
npm start
```{{execute T4}}

After the development server has started, you can [open the UI tab](https://[[HOST_SUBDOMAIN]]-3000-[[KATACODA_HOST]].environments.katacoda.com).

You should be presented with the login screen of the `create-react-app` application and you can
login as either `Alice` or `Bob`.

Note: If you're trying this locally on Windows you will need to set the environment variable as `$env:REACT_APP_LEDGER_ID="participant1"`
