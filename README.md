# Essential Skills Faculty Guide

A faculty resource for teaching the 10 Essential Skills in the **Kentucky Graduate Profile** from the Kentucky Council on Postsecondary Education (CPE). It's built by OCTC Instructional Design and uses the same branding as the [AI Literacy Faculty Playbook](https://octc-instructional-design.github.io/ai-literacy-playbook/).

## The 10 Essential Skills

Each skill has a fixed number, and the site always shows the number next to the name.

| # | Skill | Page |
|---|---|---|
| 1 | Communication | `pages/skill-01.html` |
| 2 | Critical and Creative Thinking | `pages/skill-02.html` |
| 3 | Quantitative Reasoning | `pages/skill-03.html` |
| 4 | Interpersonal Relations | `pages/skill-04.html` |
| 5 | Adaptability and Leadership | `pages/skill-05.html` |
| 6 | Professionalism | `pages/skill-06.html` |
| 7 | Civic Engagement | `pages/skill-07.html` |
| 8 | Collaboration and Teamwork | `pages/skill-08.html` (rubric) + `skill-08-1.html` … `skill-08-4.html` (indicators 8.1–8.4) |
| 9 | Knowledge Application | `pages/skill-09.html` |
| 10 | Information Literacy | `pages/skill-10.html` |

Source: [Kentucky Graduate Profile](https://cpe.ky.gov/ourwork/kygradprofile.html)

## Folder layout

```
index.html            home page with the 10 skill bars
css/styles.css        shared styles for every page
images/               OCTC logo and skill coins (skill-01.png … skill-10.png)
pages/                skill-01.html … skill-10.html (each skill's overview and rubric)
                      skill-08-1.html …   (one page per rubric row / indicator)
```

## Updating the site

- **After any change to `styles.css`**, bump the version number in the stylesheet link on every page (`styles.css?v=1` becomes `?v=2`), so browsers load the new version.
- **Reading order** for the arrows is Home, then each skill's main page followed by its indicator pages (8 → 8.1 → 8.2 → 8.3 → 8.4 → 9), then Home.
- **Skill page pattern:** the main page shows the full CPE rubric (Benchmark, Milestone, Capstone) with a link on each row. Each indicator page covers one rubric row: Benchmark to Milestone, I Can statements, What to Look For, Assessment Ideas by Discipline, and Practical Tips for Faculty.
- **Preview** the pages locally in a browser before committing. The live site updates a minute or two after a commit (look for a green check on the Actions tab).
