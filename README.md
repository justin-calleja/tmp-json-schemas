# tmp-json-schemas

If `tmp.json` has missing required properties:

`"questionRect": {},`

it should fail but:

```sh
ajv validate -s ./schemas/config.schema.json -r "./schemas/*.schema.json"  -d ./data/tmp.json
```

outputs:

```
./data/tmp.json valid
```