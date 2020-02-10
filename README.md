Prerequisites:

```
mkdocs
superfences
```

Modify ```mkdocs.yml``` as follows:

```
markdown_extensions:
    - pymdownx.superfences:
        custom_fences:
            - name  : 'fence_native'
              class : 'fence_native'
              format : !!python/name:fencenative.fence_native.fence_native_format
```

Use like this in the ```md``` files

```
 ` ```fence_native tab="Kitten" ``` `
<img src="https://placekitten.com/300/300" />
 ` ``` `
```
