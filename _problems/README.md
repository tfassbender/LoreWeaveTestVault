# Validation test problems

Fixture files designed to trigger every validation category that the LoreWeave
parser and the [lore-weave-watch](https://github.com/tfassbender/lore-weave-watch)
dashboard emit. Useful for eyeballing the live UI and for any future automated
end-to-end tests run against this vault.

| File                  | Category fired             | Severity |
|-----------------------|----------------------------|----------|
| `bad-yaml.md`         | `parse_errors`             | error    |
| `missing-type.md`     | `missing_required_fields`  | error    |
| `extra-unresolved.md` | `unresolved_links` (x2)    | error    |
| `no-title.md`         | `missing_title`            | warning  |
| `no-summary.md`       | `missing_summary`          | warning  |
| `no-schema.md`        | `missing_schema_version`   | warning  |

`bad-yaml.md` also surfaces an extra `missing_required_fields` issue as a side
effect: when frontmatter parsing fails the document has no `type`, so both
checks fire on the same file.
