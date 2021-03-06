---
title: Reviewing Pull Requests
---

# Reviewing Pull Requests

The code review process is generally regarded as a good practice and is adopted by hundreds of software projects around the world. 

It provides lot of benefits:

- **it helps spotting errors in the code**, because we all make mistakes and it can be hard to find one's own mistakes.
- **it helps improving code quality** not only by ensuring it's readable and understandable, but also by pinpointing design, performance or security issues that may have been unintentionally introduced by the author.
- **it helps spread knowledge of the code base**, because the reviewer will learn how your code works too.

{{% notice tip %}}
Reviewing is a discussion, not a to-do list. The main goal is to find the best solution by sharing different points of view.
{{% /notice %}}

## Approving Pull Requests

Maintainers are responsible for the Pull Requests they approve. The main objective of this process is to make sure that the change being reviewed does not produce undesired side effects and that it's inclusion is coherent with the project's objectives.

Here are the rules for approving a Pull Request:

1. The change must follow the [contribution guidelines][contribution-guidelines], including:
    - Coding standards
    - License & license headers
    - Proper description
2. The change must not introduce evident regressions (including breaking changes) nor substantially increase entropy, unless it's properly justified.
3. The change must provide enough value to be worth merging.

{{% notice note %}}
Fulfilling the above requirements does not automatically imply that such a contribution must be accepted.  
Conversely, non-compliant contributions **should not** be accepted.  
{{% /notice %}}

## Merging Pull Requests

A Pull Request may only be merged after the following requirements have been fulfilled:

- The change must not have any outstanding merge conflicts.
- The change has been approved by at least one maintainer (two maintainers for the [PrestaShop Core repository][prestashop-core-repository]).
- Automated checks (including automated tests) are passing.
- The change has been approved by the QA team using the "QA ✓" label, unless there's a general agreement that the change is not testable by QA.

## Stale Pull Requests

Pull Requests may be closed after 30 days of inactivity following a request for modifications.

[contribution-guidelines]: {{< ref "/1.7/contribute/contribution-guidelines/" >}}
[prestashop-core-repository]: https://github.com/PrestaShop/PrestaShop/
