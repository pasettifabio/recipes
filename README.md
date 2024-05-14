# recipes
## Steps to create a new recipe
1. Download from the internet an helm chart you like
2. Create a new folder with the name of the chart
3. Copy the content of the helm chart into the folder
4. Convert the values.yaml file in a jsonschema file called values.schema.json using some online tool like [jsonformatter](https://jsonformatter.org/yaml-to-jsonschema)
5. Run some helm commands:
    - ´´´ helm lint <chart-name> ´´´
    - ´´´ helm package <chart-name> ´´´
    - ´´´ mv <chart-name>-<chart-version>.tgz <chart-name>  ´´´
    - ´´´ helm repo index . ´´´
    - ´´´ helm repo index . --url https://pasettifabio.github.io/recipes/main ´´´