# Goalfinity Careers · Career Studio

A no-build, browser-only interview practice site using the supplied Goalfinity Careers logo. The question library includes original behavioral and scenario prompts plus role-specific prompts for 11 technology and business roles, with international-student interview practice.

## Run locally

Serve this folder with any static HTTP server (camera access generally requires `localhost` or HTTPS). For example:

```sh
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## What works in this prototype

- Select a target role and paste a job description. Local keyword matching can suggest a role and select relevant questions from the bundled library.
- Browse and filter the question library by role, skill, and prompt type.
- Record a response with the browser camera/microphone or attach a video file. The browser needs to grant camera and microphone access for recording.
- Rate each answer against the visible rubric, compare it with a role-aware answer framework, and view a report. Session ratings are stored in this browser's local storage.
- The supplied screenshot logo is cropped into `public/goalfnity-careers-logo.png` and included in the website.

## Deliberate limits

- There is no backend, account system, cloud database, or AI service. The library is a curated starter set, not an exhaustive collection of every possible interview question.
- The résumé picker displays the selected filename only. It does not parse or use résumé contents. The job description is matched locally against simple role and question keywords; this is not semantic matching.
- Videos are available for review in the active practice question, but are not uploaded to a server or saved in the session report. A recording preview is temporary and may be lost when you leave the question or close the tab.
- Scores and coaching observations are generated solely from the candidate's own rubric ratings. They do not judge spoken content, video, accent, appearance, work authorization, or hiring potential.
- The site is ready to host as a static prototype. A production service that persists résumé/video uploads or offers human-coach review needs secure storage, consent/retention controls, authentication, and an appropriate backend before collecting candidate submissions.

## Sources and question writing

The practice questions are original examples informed by common interview categories described by [Harvard FAS Career Services](https://careerservices.fas.harvard.edu/resources/interviewing/) and [CareerOneStop](https://cloudfront.careeronestop.org/Veterans/JobSearch/Interviews/common-interview-questions.aspx). They are not copied from an employer's confidential interview bank and are not predictions of a specific employer's questions.
