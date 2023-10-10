# Quasar Play Store GitHub Action

This GitHub Action connects to your [Play Store](https://play.google.com/console/u/0/developers)
by adding a step to your workflow.

```yaml
  - name: Quasar Play Store
    uses: codeeshop-oc/quasar-playstore-github-action@v2
    with:
      play_store_credentials: play-store-services.secret
      keystore_file: my-release-key.keystore
      key_store_password: 'XXXXXXXXXX'
      app_version: '1.0.0'
      package_name: 'com.app_name.com',
      alias: 'alias_name'
      app_track: 'internal'
      build_tools_version: '33.0.2'
      node_version: '18'
```

Subsequent steps in the Action can then access your github repo for quasar code.

## Inputs
### 1. `play_store_credentials`
#### Required: YES
#### Default: ''
keystore_file

### 2. `keystore_file`
#### Required: YES
#### Default: ''
keystore_file

### 3. `key_store_password`
#### Required: YES
#### Default: ''
key_store_password

### 4. `app_version`
#### Required: YES
#### Default: ''
app_version

### 5. `package_name`
#### Required: YES
#### Default: ''
package_name

### 6. `alias`
#### Required: YES
#### Default: 'alias'
alias

### 7. `app_track`
#### Required: NO
#### Default: 'internal'
app_track

### 8. `build_tools_version`
#### Required: NO
#### Default: '33.0.2'
build_tools_version

### 9. `node_version`
#### Required: NO
#### Default: '18'
node_version
