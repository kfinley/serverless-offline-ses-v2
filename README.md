# serverless-offline-ses-v2

Serverless plugin to run [aws-ses-v2-local](https://github.com/domdomegg/aws-ses-v2-local)

## Install

```
npm install serverless-offline-ses-v2
```

## Usage

### Serverless configuration

Add it to your list of plugins, and optinally custom config

serverless.yaml:

```yaml
plugins:
  - serverless-offline
  - serverless-offline-ses-v2

custom:
  serverless-offline-ses-v2:
    port: 8005
```

serverless.js / serverless.ts:

```ts
export default {
  plugins: [
    "serverless-offline",
    "serverless-offline-ses-v2",
  ],
  custom: {
    'serverless-offline-ses-v2': {
      port: 8005,
    }
  }
}
```
