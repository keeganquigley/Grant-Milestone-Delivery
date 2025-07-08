Yarn tests:

```ts
yarn run v1.22.22
$ jest
 PASS  src/__tests__/viewmodels/vc-schemas-version-history.vm.test.ts
 PASS  src/__tests__/viewmodels/login.vm.test.ts
 PASS  src/__tests__/viewmodels/schema-data-manager.vm.test.ts
 PASS  src/__tests__/viewmodels/vc-schemas-edit.vm.test.ts
 PASS  src/__tests__/viewmodels/did-list.vm.test.ts
 PASS  src/__tests__/viewmodels/vc-schemas-create.vm.test.ts
 PASS  src/__tests__/viewmodels/vc-schemas-list.vm.test.ts
 PASS  src/__tests__/viewmodels/settings.vm.test.ts
 PASS  src/__tests__/stores/auth-store.test.ts
 PASS  src/__tests__/lib/core/schemas/settings.test.ts
 PASS  src/__tests__/lib/core/schemas/auth.test.ts
 PASS  src/__tests__/stores/schema-store.test.ts
 PASS  src/__tests__/lib/core/schemas/verification.test.ts
 FAIL  src/__tests__/lib/core/web3/chain-interaction-manager.test.ts
  ● Test suite failed to run

    Cannot find module '@polkadot-api/descriptors' from 'src/lib/core/web3/chain-interaction-manager.ts'

    Require stack:
      src/lib/core/web3/chain-interaction-manager.ts
      src/__tests__/lib/core/web3/chain-interaction-manager.test.ts

    

      at Resolver._throwModNotFoundError (node_modules/jest-resolve/build/index.js:863:11)
      at Object.<anonymous> (src/lib/core/web3/chain-interaction-manager.ts:5974:27)
      at Object.<anonymous> (src/__tests__/lib/core/web3/chain-interaction-manager.test.ts:42:34)

 FAIL  src/__tests__/viewmodels/verification.vm.test.ts
  ● Test suite failed to run

    Cannot find module '@polkadot-api/descriptors' from 'src/viewmodels/verification.vm.ts'

    Require stack:
      src/viewmodels/verification.vm.ts
      src/__tests__/viewmodels/verification.vm.test.ts

    

      at Resolver._throwModNotFoundError (node_modules/jest-resolve/build/index.js:863:11)
      at Object.<anonymous> (src/viewmodels/verification.vm.ts:3303:26)
      at Object.<anonymous> (src/__tests__/viewmodels/verification.vm.test.ts:70:25)

------------------------------------|---------|----------|---------|---------|---------------------------------------------
File                                | % Stmts | % Branch | % Funcs | % Lines | Uncovered Line #s                           
------------------------------------|---------|----------|---------|---------|---------------------------------------------
All files                           |   36.95 |    25.78 |   37.06 |   36.89 |                                             
 lib/core/schemas                   |     100 |      100 |     100 |     100 |                                             
  auth.ts                           |     100 |      100 |     100 |     100 |                                             
  settings.ts                       |     100 |      100 |     100 |     100 |                                             
 lib/core/web3                      |       0 |        0 |       0 |       0 |                                             
  chain-interaction-manager.ts      |       0 |        0 |       0 |       0 | 1-473                                       
 stores                             |     100 |      100 |     100 |     100 |                                             
  auth-store.ts                     |     100 |      100 |     100 |     100 |                                             
  schema-store.ts                   |     100 |      100 |     100 |     100 |                                             
 viewmodels                         |   40.73 |    34.03 |   39.15 |   41.13 |                                             
  credentials-create.vm.ts          |       0 |        0 |       0 |       0 | 1-184                                       
  credentials-edit.vm.ts            |       0 |        0 |       0 |       0 | 3-218                                       
  credentials-list.vm.ts            |       0 |        0 |       0 |       0 | 1-55                                        
  credentials-send.vm.ts            |       0 |        0 |       0 |       0 | 1-32                                        
  credentials-utils.vm.ts           |       0 |        0 |       0 |       0 | 7-76                                        
  dashboard.vm.ts                   |       0 |      100 |       0 |       0 | 1-64                                        
  did-list.vm.ts                    |     100 |       90 |     100 |     100 | 27,60,79                                    
  login.vm.ts                       |    75.9 |       60 |   78.57 |   76.54 | 67-74,115,120,124-134,148-155               
  organization-profile-create.vm.ts |       0 |        0 |       0 |       0 | 2-55                                        
  organization-profiles.vm.ts       |       0 |        0 |       0 |       0 | 2-123                                       
  reports.vm.ts                     |       0 |        0 |       0 |       0 | 1-159                                       
  schema-data-manager.vm.ts         |   89.61 |    76.08 |      95 |   88.73 | 38,59-69,141-154                            
  settings.vm.ts                    |   94.44 |    57.14 |    90.9 |   95.91 | 59,75                                       
  user-create.vm.ts                 |       0 |        0 |       0 |       0 | 1-86                                        
  user-edit.vm.ts                   |       0 |        0 |       0 |       0 | 1-78                                        
  users.vm.ts                       |       0 |        0 |       0 |       0 | 2-95                                        
  vc-schemas-create.vm.ts           |     100 |    64.28 |     100 |     100 | 39-85                                       
  vc-schemas-edit.vm.ts             |    91.3 |    66.66 |   91.66 |   95.38 | 40,76-77                                    
  vc-schemas-list.vm.ts             |   98.41 |    83.33 |   94.11 |    98.3 | 131                                         
  vc-schemas-version-history.vm.ts  |   67.02 |    43.18 |   64.86 |   67.44 | ...-390,396-399,404-411,427-429,461,545-546 
  verification.vm.ts                |       0 |        0 |       0 |       0 | 1-341                                       
------------------------------------|---------|----------|---------|---------|---------------------------------------------
Jest: "src/lib/core/web3/chain-interaction-manager.ts" coverage threshold for statements (90%) not met: 0%
Jest: "src/lib/core/web3/chain-interaction-manager.ts" coverage threshold for branches (65%) not met: 0%
Jest: "src/lib/core/web3/chain-interaction-manager.ts" coverage threshold for lines (90%) not met: 0%
Jest: "src/lib/core/web3/chain-interaction-manager.ts" coverage threshold for functions (90%) not met: 0%
Test Suites: 2 failed, 13 passed, 15 total
Tests:       1 skipped, 114 passed, 115 total
Snapshots:   0 total
Time:        5.689 s
Ran all test suites.
error Command failed with exit code 1.
```
