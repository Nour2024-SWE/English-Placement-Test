# English Placement Test 

A lightweight, browser-based English Placement Test for evaluating students' English proficiency through listening, grammar, vocabulary, reading, and advanced-structure questions.

The project is designed as a standalone front-end application. It requires no server, database, build process, or external framework.

## Project Overview

The application provides a complete testing workflow:

- Student identification using full name and student ID.
- A 25-question randomized English placement examination.
- Listening comprehension, grammar and structure, vocabulary, reading comprehension, and advanced structures.
- Interactive question cards with answer selection and progress tracking.
- Automatic grading and percentage calculation.
- CEFR-style level estimation from A1 to C1.
- Bilingual English/Arabic result descriptions.
- Detailed answer review after submission.
- Browser-based result storage using LocalStorage.
- Teacher/admin view of recent stored results.
- CSV export with UTF-8 encoding and Arabic column headings.
- Print-friendly results for saving or printing from the browser.

## Examination Structure

| Section | Question Range | Main Skill |
|---|---:|---|
| Listening Comprehension | 1–5 | Understanding spoken English |
| Grammar and Structure | 6–12 | Sentence formation and grammar |
| Vocabulary | 13–17 | Word meaning and usage |
| Reading Comprehension | 18–22 | Understanding written passages |
| Advanced Structures | 23–25 | Higher-level grammar and usage |

Questions are selected and displayed dynamically by the application.

## CEFR-Style Level Mapping

| Score out of 25 | Estimated Level |
|---:|---|
| 0–7 | A1 |
| 8–13 | A2 |
| 14–18 | B1 |
| 19–22 | B2 |
| 23–25 | C1 |

The levels are application-defined estimates and should not be treated as an official CEFR certification.

## Repository Structure

```text
english-placement-test/
├── index.html
├── neu-logo-site.png
├── README.md
├── LICENSE
└── .gitignore
```

## Technology Stack

- HTML5
- CSS3
- Vanilla JavaScript
- Browser LocalStorage
- Browser Text-to-Speech API, where supported
- CSV export through the browser Blob API

No installation of Python, Node.js, a database, or a package manager is required.

## Getting Started

### Option 1: Open Locally

1. Download or clone the repository.
2. Open `index.html` in a modern web browser.
3. Enter the student's name and ID.
4. Complete all 25 questions.
5. Submit the examination to calculate the result.

### Option 2: Run with a Local HTTP Server

A local server is useful when browser security restrictions affect audio or other browser APIs.

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Student Workflow

1. Enter the required student information.
2. Start the test.
3. Select one answer for each question.
4. Use the progress bar to monitor completion.
5. Submit only after all questions have been answered.
6. Review the score, percentage, estimated level, and answer-by-answer feedback.
7. Print or save the result if required.

## Teacher and Admin Workflow

The application includes a local admin/results panel that can:

- Display the number of stored attempts.
- Show recent student results.
- View the date, student name, ID, score, percentage, and estimated level.
- Export the stored results as a CSV file.
- Clear locally stored results when appropriate.

### Data Storage Notice

Results are stored in the browser's LocalStorage under:

```text
neu_english_placement_results
```

This means the data is local to the browser and device. LocalStorage is not a replacement for a secure central student information system. For production deployment, use authentication, a server-side database, access controls, backups, and privacy protections.

## GitHub Pages Deployment

The project can be published as a static website:

1. Push the repository to GitHub.
2. Open the repository's **Settings**.
3. Select **Pages**.
4. Choose the deployment branch and root folder.
5. Save the configuration.
6. Open the generated GitHub Pages URL.

## Suggested Repository Topics

```text
english-placement-test
language-assessment
english-proficiency
cefr
education
javascript
html
css
e-learning
assessment-tool
```

## Limitations and Future Improvements

Potential extensions include:

- Server-side result storage.
- Secure teacher authentication.
- Question-bank management.
- Multiple test versions and difficulty levels.
- Randomized question pools with configurable section weights.
- More accessible keyboard and screen-reader interactions.
- Export to PDF and XLSX through a backend service.
- Analytics dashboards for class-level performance.
- Optional timer and test-attempt controls.
- Internationalization for additional languages.

## Academic and Educational Use

This repository is suitable for educational demonstrations, placement-test prototypes, classroom assessment, and front-end learning projects. Before using it for high-stakes placement decisions, validate the questions, scoring rules, accessibility, reliability, and privacy requirements with qualified language-assessment staff.

## License

Released under the MIT License. See [LICENSE](LICENSE).

## Author

Replace this line with the project owner, department, university, or organization name before publishing.
