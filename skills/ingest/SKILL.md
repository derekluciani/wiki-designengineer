---
name: wiki-injest
description: Run this skill when the user asks to injest a new document from the /raw directory.
---

Use this skill as an instruction set. Follow the workflow in order.

## Workflow

1. Read the new source document mentioned by the user.
2. Present _key takeaways_ to the user.
3. Ask the user if the _key takeaways_ are sufficient enough to be added as a new _topic_ HTML file in the /wiki directory. Once the user gives an approval, move onto the next step.
4. Create the new _topic_ html page (using a copy of `@page_template.html` and applying the `{NAME}_topic.html` naming convention).
5. Update the `index.html` page with a new _topic_ `listing`.
6. Update all cross-references and related pages across the wiki.
7. Append an `entry` to the `log.html` file. Ensure the latest entry is added to the top of the list.
