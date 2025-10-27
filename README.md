#

```
env LOG_LEVEL=debug GITHUB_COM_TOKEN="$(gh auth token)" node ~/workspaces/renovate/dist/renovate.js --token "$(gh auth token)" --platform local --onboarding=false --require-config=optional

env LOG_LEVEL=debug GITHUB_COM_TOKEN="$(gh auth token)" node ~/workspaces/renovate/dist/renovate.js --token "$(gh auth token)" --onboarding=false --require-config=optional JamieTanna-Mend-testing/renovate-iss-38324
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

##

- Repo does not `Automatically delete head branches`
- 1ccc6711c57ae3134d4a4b02475b54dabc55acd6 contains everything ready to test

```json
DEBUG: packageFiles with updates (repository=JamieTanna-Mend-testing/renovate-iss-38324, baseBranch=main)
       "config": {
         "npm": [
           {
             "deps": [
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
                     "pendingChecks": true,
                     "libYears": 0.0958863077435312,
                     "branchName": "renovate/all-minor-patch"
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
             ],
             "extractedConstraints": {"npm": ">=7"},
             "managerData": {
               "hasPackageManager": false,
               "npmLock": "package-lock.json",
               "yarnZeroInstall": false,
               "npmrcFileName": null
             },
             "skipInstalls": true,
             "packageFile": "package.json",
             "lockFiles": ["package-lock.json"]
           }
         ],
         "nvm": [
           {
             "deps": [
               {
                 "depName": "node",
                 "currentValue": "22.19.0",
                 "datasource": "node-version",
                 "updates": [
                   {
                     "bucket": "non-major",
                     "newVersion": "v22.21.0",
                     "newValue": "22.21.0",
                     "releaseTimestamp": "2025-10-20T00:00:00.000Z",
                     "newVersionAgeInDays": 7,
                     "newMajor": 22,
                     "newMinor": 21,
                     "newPatch": 0,
                     "updateType": "minor",
                     "isBreaking": false,
                     "libYears": 0.14520547945205478,
                     "branchName": "renovate/all-minor-patch"
                   }
                 ],
                 "packageName": "node",
                 "versioning": "node",
                 "warnings": [],
                 "sourceUrl": "https://github.com/nodejs/node",
                 "registryUrl": "https://nodejs.org/dist",
                 "homepage": "https://nodejs.org",
                 "currentVersion": "v22.19.0",
                 "currentVersionTimestamp": "2025-08-28T00:00:00.000Z",
                 "currentVersionAgeInDays": 60,
                 "isSingleVersion": true,
                 "fixedVersion": "22.19.0"
               }
             ],
             "packageFile": ".nvmrc"
           }
         ]
       }
```
