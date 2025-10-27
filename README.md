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
- 717020200dca96230429494b02a4f446435956f6 contains everything ready to test

1. Check out 717020200dca96230429494b02a4f446435956f6
1. Run Renovate (on a week day)
  1. `Update Node.js to v22.21.0` is "Awaiting Schedule", due to `schedule:weekends`

<details>



```json
DEBUG: packageFiles with updates (repository=JamieTanna-Mend-testing/renovate-iss-38324, baseBranch=main)
       "config": {
         "npm": [
           {                                                                                                                                                                                                                                                "deps": [
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

</details>

1. Tick `Update Node.js to v22.21.0`
1. Run Renovate
  - PR `Update Node.js to v22.21.0` is created as `renovate/all-minor-patch`

<details>

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

</details>

1. Merge PR and **do not delete branch**
  - As commit ``
1. Run Renovate again (on a weekend)
  - Or with `RENOVATE_IGNORE_PRESETS=schedule:weekends`
  - It re-uses branch

<details>


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
                     "pendingChecks": true,                   <<<<<<<<<<<<<<<<<<<<<
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
                 "currentValue": "22.21.0",
                 "datasource": "node-version",
                 "updates": [],
                 "packageName": "node",
                 "versioning": "node",
                 "warnings": [],
                 "sourceUrl": "https://github.com/nodejs/node",
                 "registryUrl": "https://nodejs.org/dist",
                 "homepage": "https://nodejs.org",
                 "currentVersion": "v22.21.0",
                 "currentVersionTimestamp": "2025-10-20T00:00:00.000Z",
                 "currentVersionAgeInDays": 7,
                 "fixedVersion": "22.21.0"
               }
             ],
             "packageFile": ".nvmrc"
           }
         ]
       }

DEBUG: Update has not passed minimum release age (repository=JamieTanna-Mend-testing/renovate-iss-38324, branch=renovate/all-minor-patch)
       "depName": "contentful",
       "timeElapsed": 566604171,
       "minimumReleaseAge": "300 days"

DEBUG: Branch summary (repository=JamieTanna-Mend-testing/renovate-iss-38324)
       "cacheModified": undefined,
       "baseBranches": [{"branchName": "main", "sha": "8cf546fc49fa607414f507302fb65656b69a7f9a"}],
       "branches": [
         {
           "automerge": false,
           "baseBranch": "main",
           "baseBranchSha": "8cf546fc49fa607414f507302fb65656b69a7f9a",
           "branchName": "renovate/all-minor-patch",
           "branchSha": "150ae5ad70eaad4be4fd5a244059d0803ee64b7e",
           "isModified": false,
           "isPristine": true
         }
       ],
       "defaultBranch": "main",
       "inactiveBranches": []
DEBUG: branches info extended (repository=JamieTanna-Mend-testing/renovate-iss-38324)
       "branchesInformation": [
         {
           "branchName": "renovate/all-minor-patch",
           "prNo": 5,
           "prTitle": "Update dependency contentful to v11.8.7",
           "result": "done",
           "upgrades": [
             {
               "datasource": "npm",
               "depName": "contentful",
               "displayPending": "",
               "fixedVersion": "11.7.19",
               "currentVersion": "11.7.19",
               "currentValue": "^11.7.19",
               "newValue": "^11.7.19",
               "newVersion": "11.8.7",
               "packageFile": "package.json",
               "updateType": "minor",
               "packageName": "contentful"
             }
           ]
         }
       ]
```

</details>
