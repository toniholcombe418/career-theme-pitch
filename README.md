# Career Theme Pitch

A Claude skill that helps job seekers show a hiring team, fast, that they have already solved the problem the job exists to solve.

Most job search advice starts with the resume. This skill starts with you. It interviews you like a podcast guest, finds the theme that runs through your career, and then turns that theme into a pitch built around the business problem in a real job posting.

Created by Toni Holcombe, host of [Tell Me About a Time](https://tellmeaboutatime.io), a podcast that interviews people who are currently looking for work.

## What it does

1. **Interviews you.** Claude asks one question at a time about your work stories, the way a podcast host would, with a countdown so you know how many are left. It pushes past vague answers until each story has what happened, how you handled it, and the result.
2. **Names your theme.** Claude finds the move you make again and again across jobs, names it in your own words, and checks that it rings true to you.
3. **Reads your resume and LinkedIn profile.** It flags stories your documents leave out, and results you never mentioned.
4. **Finds the business problem.** For each job posting you share, Claude answers one question: what goes wrong for this company if this seat stays empty?
5. **Aligns your accomplishments.** It matches your strongest stories to that problem and tells you honestly where the gaps are.
6. **Writes three resume summaries.** Short, built on facts you confirmed, and each one names the business problem from the posting.
7. **Offers to rewrite your LinkedIn profile.** Headline, About, experience, and skills, written for how recruiters and LinkedIn's AI hiring tools actually read profiles.
8. **Offers to build a master resume.** A general version for your target role, using standard section headers that applicant tracking systems (ATS) can read.
9. **Offers a tailored resume for each posting.** It starts from the master resume and changes the summary, bullet order, and skills to fit each job. Paste a new posting at any time to get another.

Claude names each step as it starts and tells you what is still to come, so nothing gets skipped.

The rules behind the summaries and the LinkedIn rewrite come from research on how recruiters and LinkedIn's AI tools screen candidates. See `references/screening-research.md` for the sources and how strong each one is.

## What you need

- About 45 to 60 minutes for the full process
- Your resume, as a PDF or Word file
- Your LinkedIn profile open on a computer, so you can copy each section
- One to five job postings you want to apply for (you can add these later in the conversation)

## Install it

### Claude.ai or the Claude desktop app

Claude needs the skill as a ZIP file of a folder named exactly `career-theme-pitch`. GitHub's download names the folder differently, so follow these steps.

1. On this page, click the green **Code** button, then **Download ZIP**.
2. Unzip the file. You will get a folder named something like `career-theme-pitch-main`.
3. Rename that folder to `career-theme-pitch`.
4. Compress the renamed folder into a ZIP file.
5. In Claude, open **Customize**, then **Skills**.
6. Click the **+** button, then **Create skill**, then **Upload a skill**.
7. Choose your ZIP file.

If the upload fails, check that the folder name is exactly `career-theme-pitch` and that `SKILL.md` sits directly inside it. Menu names can change, so see Anthropic's guide, [Use skills in Claude](https://support.claude.com/en/articles/12512180-use-skills-in-claude), if your screen looks different.

Custom skills you upload are private to your account.

### Claude Code

Copy the `career-theme-pitch` folder into your personal skills folder at `~/.claude/skills/`.

## Use it

Start a new chat and say something like:

- "Help me with my job search."
- "I want to figure out what makes me different as a candidate."
- "Help me rewrite my LinkedIn profile for content director roles."

Claude will recognize when the skill applies. You do not need to name it.

### Tips for better results

- **Answer in your own words.** Talk the way you would to someone at a networking event. Polished answers hide the details that make your theme clear.
- **Give specifics.** Numbers, names of projects, and what changed afterward make the strongest stories. If you do not remember an exact number, a rough one is fine. Say it is an estimate.
- **Push back.** If the theme Claude names does not feel like you, say so. The skill will ask more questions and try again.
- **Check every fact.** Claude marks anything missing in [brackets]. Fill those in before you use any of the writing.
- **Test your summaries.** You get three versions on purpose. Try different ones with different applications and notice which get responses.

### Privacy

Share only what you are comfortable sharing. The skill tells Claude to leave out personal details such as age, health, family, and legal matters unless you ask to include them. Do not paste government ID numbers, account numbers, or other sensitive data.

## What is in this repo

```
career-theme-pitch/
├── README.md                          This file
├── SKILL.md                           Instructions Claude follows
└── references/
    └── screening-research.md          Research on how resumes and profiles get screened
```

## A note on the research

Some of the research is strong, such as Harvard Business School's Hidden Workers report. Some is anecdotal, such as recruiter posts on Reddit. Some comes from LinkedIn's own product pages and demos, which may not match how the tools behave in every case. The research file rates each source so you can weigh it yourself. Treat the problem-first summary as a strong idea to test, not a guarantee.
