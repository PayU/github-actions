# PayU Shared resources for GitHub Actions

## GitHub workflows for Maven

### verify

In order to use, please create in project:

```
.github/workflows/maven-verify.yml
```

with example content:

```yaml
#  Copyright 2021 PayU
#
#  Licensed under the Apache License, Version 2.0 (the "License");
#  you may not use this file except in compliance with the License.
#  You may obtain a copy of the License at
#
#  http://www.apache.org/licenses/LICENSE-2.0
#
#  Unless required by applicable law or agreed to in writing, software
#  distributed under the License is distributed on an "AS IS" BASIS,
#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
#  See the License for the specific language governing permissions and
#  limitations under the License.

name: Verify

on:
  push:
  pull_request:

jobs:

  # verify by maven
  verify:
    uses: PayU/github-actions/.github/workflows/maven-verify.yml@v1
```
