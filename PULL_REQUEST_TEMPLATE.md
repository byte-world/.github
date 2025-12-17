## Summary
Describe your changes.

## Checklist
- [ ] Policy compliant
- [ ] Tested
- [ ] Documented

## Impact
Low / Medium / High
```

---

## workflows/org-ci.yml

```yml
name: Org Policy CI
on:
  pull_request:
  push:

jobs:
  lint:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Basic validation
        run: echo "Org-level CI check passed"
```

© Byte World — Community Governed, Sponsor Neutral
