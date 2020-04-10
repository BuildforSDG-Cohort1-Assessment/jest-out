# jest-out
This action sends the Jest tests summary to our backend API

## Inputs

### `challenge`

**Required** The challenge in the assessment that Jest ran and needs to report on.

### `lang`

**Required** The primary language with which the developer coded the solution being tested

### `server`

**Required** The base backend API endpoint to send the report data to . Default is `"https://us-central1-buildforsdg.cloudfunctions.net"`.

## Example Usage

```bash
- name: Report Tests
  uses: BuildforSDG-Cohort1-Assessment/jest-out@v1
  with:
    challenge: ch-2
    lang: python
```

