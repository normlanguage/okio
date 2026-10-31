# Norm package template

Use this repository template for every publishable Norm package.

Replace `example_package` in `module.norm`, add source files under `src/`, and keep the generated root `SKILL.md` committed with each release.

## Required workflow

1. Declare the module and dependencies in `module.norm`.
2. Put every public declaration under `src/` and document it with `@Document`.
3. Generate the root Skill with `norm docs . --output build/api --skill SKILL.md --strict`.
4. Run `scripts/validate-package.ps1` and the package tests.
5. Release the package and `SKILL.md` from the same immutable tag.

The Registry stores only package ownership. API facts and Skill content remain in this repository.

[License](LICENSE)
