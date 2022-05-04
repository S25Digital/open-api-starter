# open-api-starter
The starter open api documentation project

This is a starter repo to provide a  structure for the api documentation using Open API v3 specification. The src folder is divided into sub-folders.

- responses: hold the structure and schema for responses
- paramters: hold the structure and schema of the query and route parameters
- resources: hold the structures for routes related to the resources
- schemas: hold the schema for the reusuable components

api.yaml file is the main file where everything is used. You need to build the repository to generate the final file.

## how to build
Use the following command to build the repo and generate the final open api spec file and html file

```
npm run build
```

The repo uses the follwoing projects:
- swagger-cli: to generate the final api.yaml file. This will combine all the files into one file.
- @stoplight/spectral-cli: used to lint and verify the structure of the final api.yaml file generate by the above step.
- redoc-cli: to generate the html file from the final api.yaml.
