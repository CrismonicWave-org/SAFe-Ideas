# SAFe-Ideas

A repo of reusable templates for a project using Scaled Agile (SAFe) specifically Lean Portfolio Management.

Here is the Hypothesis: In the world of Lean Portfolio Management, Product Management and Project Management have a set of tools that they use to manage the Agile Projects.  Examples would be Jira or VersionOne or Ralley.  These tools do a great job of capturing the Epics, Capabilities and Features as well as the Stories, yet they do so often highly optimized for Product Management and NOT the Developers whom must ultimately consume these artifacts. So, the premise of these ideas are:

- Craft the EPIC, Capabilitiy and Feature as a set of Markdown documents in a Github or Gitlab repository.
  - Why: Developers are often the peeps who are ultimately maintaining these.  Lets have them do so in VS Code instead of the Web Based tools.
  - Why: These artifacts need scrutiny and this idea treats the artifacts excatly like they are Code.  Pull Requests/Merge Requests and "Code" reviews shold be stringant.
  - Why: Since this is now treated as Source Code, Linting rules and Code Scans can be used to ensure that inapproriate data is not escaping.  True story, I;ve seen in a Story in Jira a GitLab Personal Access Token in the story.  That security violation endured for several years.
- In your Agile Practice Management tool of choice, the Product Management peeps can keep the amount of data in the Tool to a minimum and use links to the repository's latest version so the repository becomes the Single Source of Truth.
  - Why: Yes it is true that Product Managers often are resitant to using the tools that the developers use.  OK, I get that, but again, the Developers are the peeps whom need to comsume this information.  Indeed, in the code, if you want traceability, it is easy to bake that into the actual Source Code repository readme.md files tracing a commit back to the story by linking to the story markdown.
- Finally, it is apparent to me that the Microsofts (GitHub) and GitLab are moving towards providing One Stop Shop for Software Delivery including Agile Practice Management all baked into the repository.  I predict that eventually, GitHub will provide tooling for Product Managers, Program Managers, Project Managers and the Developers ALL in one spot.  This idea on how to manage these artifacts is my initial implementation of what I believe is only a matter of time.

Feel free to reach out to me at kencrismon@crismonicwave.com and we can chat, argue, debate and go from there.

I want opinion, alternate ideas etcetera as there has to be a better way.  I think this might be one idea, there are certainly others.

# Maintenance of Markdown Ideas

- I use VS Code as my preferred editor for manipulating and maintaning Markdown.
- I use the two following VS Code Extensions
  - [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)
    - In the Templates, you will see numbers and descriptions for the Table Of Contents.  To acomplish this, after installing the Plugin, I execute from the command pallete the command `section` which will insert numbers into the \#\# Headers automatically and I set the Update TOC upon save.

    Note that as you add new \#\# sections it is suggested that you quickly re-run the `section` command from the VS Code Pallete which will add the section numbers to the document and upon saving will update the Table of Contents.

    Edit away and your TOC should follow your document design.
  - [Markdown Lint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint)
    - I find this one helpful but certainly you can disable it.  I try to strictly use it.
