# Zilch RFCs

This repository contains Request For Comments (RFC) for both Zilch and N\*.
Having RFCs public allows anyone to take part in the discussions related to this language, or even propose new changes and make it evolve.

## What are RFCs for

A RFC is a formal document whose purpose is to discuss new features, syntax changes, API changes, etc.
Individual bug fixes made to the Zilch compiler should *not* be formalized as RFCs, unless deemed necessary by the maintainers.
If this is the case, you will be redirected to this repository for further information.

**Note:** a change to the internal compiler API may not automatically be within the scope of a RFC. 
If you are unsure, feel free to open an issue here to ask before writing a complete RFC.

## Writing a new RFC

There is a RFC template named [`0000-template.md`](./rfcs/0000-template.md) available in this repository.
This template **must** be used as the basis of your RFC.
Any RFC submitted which does not follow this template may simply be refused.
Please also note that any PR whose RFC does not comply with the current goals of Zilch may also be closed.
If you are unsure about those goals, or whether your proposal fits them, please open an issue here and ask.
This will save you the time that would have been invested in writing a complete off-topic RFC.

Copy the `0000-template.md` to the `rfcs` folder, and give it a proper name.
This name must be short and descriptive of your RFC.
As a quick example, a RFC about adding named type class instances may be named `0000-named-instances.md`.
Do not change the `0000-`, as this will be used later when you issue a PR.

You can then start writing your RFC by filling the blanks in the template.
Do not fill the beginning table: it will be filled by contributors once your RFC is accepted (or refused).

After you finished writing a draft of your RFC, open a [pull request](https://github.com/zilch-lang/rfc/compare).
The pull request must contain a quick summary of your proposed changes, along with a link to the rendered markdown file.
Be aware that your RFC will be heavily criticized/discussed.
If you are not ready to receive such comments, submitting a RFC might not be a good idea.
Try to keep discussions/changes inside the pull request, as this will allow keeping track of progress.
If discussion happens outside of the pull request, please include a summary of everything discussed.

## Amending RFCs

Sometimes, RFC have to be superseded by other RFCs.
In such case, the new RFC should include a link to the original RFC in a comment at the very top, under the header (something like `> This RFC supersedes [RFC#WXYZ](./WXYZ-rfcname.md)`).
As a matter of organisation, the replaced RFC should also be annotated with `> This RFC has been replaced by [RFC#WXYZ](./WXYZ-rfcname.md)`.

## RFC lifecycle

This sections describes what stages a RFC may undergo before being merged.
This lifecycle may not be strictly followed in some special cases, but it is strongly advised to.

1. The author submits an original draft as a pull request.
2. RFC revision: discussions happen inside the pull request, some changes are made to the RFC, feedback is given.
3. The RFC will be judged stable enough at some point by maintainers. When this stage is reached, only minor changes must be made to the RFC. If a major change has to be done, the RFC returns to stage 2.
4. After some time (usually 1-3 weeks, although this may last longer), the RFC is frozen, discussion is limited to maintainers and the author of the pull request.
5. The RFC is then either accepted or refused.
  When accepted, the RFC will be merged and the header will be filled. The author does not need to be involved in adding the proposed feature to the project, albeit recommanded.
  If refused, the PR will be closed by a comment explaining the reasons for the refusal.

## License

All redacted documents present in this repository are licensed under the MIT license.
