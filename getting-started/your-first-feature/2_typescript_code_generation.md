Remember that we interface with the Daml model from the UI components using generated TypeScript. Since we have changed our Daml code, we also need to rerun the TypeScript code generator. Run the following commands in terminal 1 by clicking on the code below:

```
cd create-daml-app
daml build
daml codegen js .daml/dist/create-daml-app-0.1.0.dar -o ui/daml.js
```{{execute T1}}

The result is an up-to-date TypeScript interface to our Daml model, in particular to the new `Message` template and `SendMessage` choice.

*Only after the above commands have been executed run `npm` to install the project dependencies by
clicking on the code below*. To make sure that `npm` picks up the newly generated JavaScript code, we
have to run the following command in the ui directory:

```
cd create-daml-app/ui
npm install --force --frozen-lockfile
```{{execute T2}}

Once that command finishes we can start implementing our messaging feature in the UI!
