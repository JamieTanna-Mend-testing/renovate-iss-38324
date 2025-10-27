```
env LOG_LEVEL=debug GITHUB_COM_TOKEN="$(gh auth token)" node ~/workspaces/renovate/dist/renovate.js --token "$(gh auth token)" --platform local --onboarding=false --require-config=optional
```


```json
{
  "depType": "dependencies",
  "depName": "contentful",
  "currentValue": "^11.7.19",
  "datasource": "npm",
  "prettyDepType": "dependency",
  "lockedVersion": "11.7.19",
  "updates": [
    {
      "bucket": "non-major",
      "newVersion": "11.8.7",
      "newValue": "^11.7.19",
      "releaseTimestamp": "2025-10-21T00:09:39.778Z",
      "newVersionAgeInDays": 6,
      "newMajor": 11,
      "newMinor": 8,
      "newPatch": 7,
      "updateType": "minor",
      "isBreaking": false,
      "isRange": true,
      "isLockfileUpdate": true,
      "pendingChecks": true,                           <<<<<<<<<
      "libYears": 0.0958863077435312,
      "branchName": "renovate/contentful-11.x-lockfile"
    }
  ],
  "packageName": "contentful",
  "versioning": "npm",
  "warnings": [],
  "sourceUrl": "https://github.com/contentful/contentful.js",
  "registryUrl": "https://registry.npmjs.org",
  "homepage": "https://www.contentful.com/developers/documentation/content-delivery-api/",
  "mostRecentTimestamp": "2025-10-21T00:09:39.778Z",
  "currentVersion": "11.7.19",
  "currentVersionTimestamp": "2025-09-16T00:11:49.177Z",
  "currentVersionAgeInDays": 41,
  "isSingleVersion": true,
  "fixedVersion": "11.7.19"
}
```
