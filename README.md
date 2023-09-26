# Conviso AST
Run Conviso AST in your repository and assess the results in Conviso Platform.
More information [here](https://docs.convisoappsec.com/cli/ast)

## Usage

> ##### This action requires [Conviso AST Action](https://github.com/marketplace/actions/conviso-ast)

```yaml
-   name: Conviso AST
    on: push
    jobs: 
        conviso-ast:
            runs-on: ubuntu-latest
            steps: 
                uses: convisoappsec/conviso-ast@v1
                env:
                    CONVISO_API_KEY: ${{ secrets.CONVISO_API_KEY }}
                with:
                    args: ""
```

----

### Environment variables
- `CONVIO_API_KEY` (required) - Conviso API Key 

### Inputs
- `args` (optional) - Additional arguments to set

### License
See the [LICENSE](LICENSE) FILE for more details.