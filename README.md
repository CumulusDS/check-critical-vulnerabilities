[![Create Release][release-badge]][release-url]
[![Import Labels][import-labels-badge]][import-labels-url]
[![Sync Labels][sync-labels-badge]][sync-labels-url]
[![PR AutoLabeler][autolabeler-badge]][autolabeler-url]
[![Assigner][assigner-badge]][assigner-url]

Checks repository for any critical vulnerabilities, and if found, fails CI.

### Inputs
#### `token`
Token with permissions to check repository for vulnerabilities

#### `level`
Override failing level for action.
Default: `CRITICAL`

#### `fail`
Override failure on found vulnerabilities.  Set to `false` to disable action failure
Default: `true`

### Example usage
```yaml
      - name: Check for failing vulnerabilities
        uses: CumulusDS/check-critical-vulnerabilities@v1
        with:
          token: ${{ secrets.APPROPRIATE_TOKEN }}
```


[release-badge]: https://github.com/CumulusDS/check-critical-vulnerabilities/actions/workflows/release.yml/badge.svg
[release-url]: https://github.com/CumulusDS/check-critical-vulnerabilities/actions/workflows/release.yml
[import-labels-badge]: https://github.com/CumulusDS/check-critical-vulnerabilities/actions/workflows/labels_import.yml/badge.svg
[import-labels-url]: https://github.com/CumulusDS/check-critical-vulnerabilities/actions/workflows/labels_import.yml
[sync-labels-badge]: https://github.com/CumulusDS/check-critical-vulnerabilities/actions/workflows/labels_sync.yml/badge.svg
[sync-labels-url]: https://github.com/CumulusDS/check-critical-vulnerabilities/actions/workflows/labels_sync.yml
[autolabeler-badge]: https://github.com/CumulusDS/check-critical-vulnerabilities/actions/workflows/autolabeler.yml/badge.svg
[autolabeler-url]: https://github.com/CumulusDS/check-critical-vulnerabilities/actions/workflows/autolabeler.yml
[assigner-badge]: https://github.com/CumulusDS/check-critical-vulnerabilities/actions/workflows/assign.yml/badge.svg
[assigner-url]: https://github.com/CumulusDS/check-critical-vulnerabilities/actions/workflows/assign.yml
