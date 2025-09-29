# testing-glean




| ID  | Test Name      | # | Status| Notes                  |
|-----|----------------|---|-------|------------------------|
| 1   | XYZ            | 1 | FAIL  | Version file|
| 2   | XYZ            | 2 | FAIL  |   |
| 3   | XYZ            | 3 | FAIL  |   |
| 4   | Commit v Docs  | 1 | Open  |     |
| 5   | Commit v Docs  | 2 | Open  |     |
| 6   | Commit v Docs  | 3 | Open  |      |
| 7   | Biz Reqs       | 1 | Open  |     |
| 8   | Biz Reqs       | 2 | Open  |     |
| 9   | Biz Reqs       | 3 | Open  |      |
| 10  | Biz Policy     | 1 | Open  |     |
| 11  | Biz Policy     | 2 | Open  |    |
| 12  | Biz Policy     | 3 | Open  |   |
| 13  | Permissions    | 1 | Open  |     |
| 14  | Permissions    | 2 | Open  |    |
| 15  | Permissions    | 3 | Open  |     |


Question 1:

Jerry wanted to know “in which version a specific feature (XYZ) was released.”

Answer:

Notes:

This seems to only be possible if the version number (XYZ) is specifically entered in a commit message, which is not typical for developers. Conclusion: no, unless verbose and strict commit message standards are implemented.

Question 2:
He also wanted to know if the answer to the previous question would come from a commit message or documentation associated with a particular repository.

In tests, Glean prefers documentation such as Changelogs, although it will search commit messages as well as described above.

Question 3:

If he gets into a new code base and needs to derive the business requirements, can he extract business functionality from the repository?

Yes, this worked well assuming enough detail exists in the README, commit messages, or other documentation files. It will not work if the business functionality is only in the code files themselves (in which case it would require the Glean Code Tool).

Question 4:

“What is the business policy associated with the user account login; what are the different roles considered in the system?”

Question 5:

“What are the permissions associated with this particular role?”

Both of these would require the Glean Code Tool, which I’d like to explore more tomorrow.