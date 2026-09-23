# Security policy

This is the default policy for every repository in the Gubernaut organisation that does not carry
its own. The code's own policy, with what counts as a vulnerability in a control layer and what is
a documented limit instead, is in the main repository:
[thegubernaut/gubernaut/SECURITY.md](https://github.com/thegubernaut/gubernaut/blob/main/SECURITY.md).

## Reporting a vulnerability

**Do not open a public issue for a security problem.**

Use GitHub's [private vulnerability reporting](https://github.com/thegubernaut/gubernaut/security/advisories/new)
on the main repository, or email **contact@gubernaut.com** with `SECURITY` in the subject.
Include the repository, the version, what you expected, what happened, and a minimal
reproduction if you have one.

This is a small project. You will get an acknowledgement within a few days; if you have not heard
back in a week, send a reminder. Report privately, allow a reasonable window for a fix, and you
will be credited in the advisory unless you would rather not be.

## The validation record

[Gubernaut_Validation](https://github.com/thegubernaut/Gubernaut_Validation) holds research data,
not running code. Its data is sealed by `SHA256SUMS`, an OpenTimestamps proof and a Zenodo DOI.
A file that fails the seal, or a published number that does not recompute from the record, is an
integrity report: open an ordinary issue there, because the whole point of the record is that
anyone can check it in public.
