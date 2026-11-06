# Contributing to KalpaXi

Thank you for helping KalpaXi. Engineers, developers, designers, testers and
students are all welcome.

## Ways to help

| Contribution | How |
|---|---|
| **Report a bug** | [Open a bug report](https://github.com/KalpaXi/KalpaXi_V2/issues/new/choose) |
| **Suggest a feature** | [Open a feature request](https://github.com/KalpaXi/KalpaXi_V2/issues/new/choose) |
| **Validation case** | Compare a KalpaXi result with a hand calculation, textbook answer or test data, and share it. These are especially valuable |
| **Documentation** | Improve the guides in the `docs/` folder, fix mistakes, add screenshots |
| **Code** | Fix a bug or build a feature (see below) |
| **Questions / feedback** | Email admin@kalpaxi.in |

## Reporting bugs

- Check the [existing issues](https://github.com/KalpaXi/KalpaXi_V2/issues) first.
- Use the bug report form. Include the KalpaXi version, your operating system, the steps to reproduce and screenshots.
- Do **not** attach confidential models. Make a small simplified model that shows the problem.
- Security problems: **do not open a public issue**. See `SECURITY.md`.

## Contributing code

1. Discuss larger changes in an issue first, so work isn't duplicated.
2. Fork the repository and create a branch: `fix/short-description` or `feature/short-description`.
3. Keep each pull request to **one** change.
4. Follow the existing code style:
   - Python: PEP 8, clear names, comments for engineering formulas with their source
   - JavaScript / TypeScript: follow the style of the surrounding code
5. For anything that changes analysis results, include a test or validation case showing the result is correct.
6. Write clear commit messages, e.g. `Fix fillet failure on small edges`.
7. Open a pull request and fill in the template.

## Contributor Licence Agreement (CLA)

Before your first pull request can be merged, you must agree to the
**KalpaXi Contributor Licence Agreement** in `CLA.md`, by ticking the box in the
pull-request template.

In short: you confirm that you wrote the contribution (or have the right to
submit it), and you allow the KalpaXi project to distribute it under the
AGPL v3 and under other licences in the future. You keep the copyright in your work.

## Engineering contributions

- State the theory and the reference (book, standard, paper) behind any formula.
- Use SI units, and say which units a value uses.
- Do not copy tables from paid standards (ISO, ASTM, FKM etc.) into the code or
  documentation. Implement the method and cite the standard instead.

## Code of conduct

Everyone taking part must follow the `CODE_OF_CONDUCT.md`.
