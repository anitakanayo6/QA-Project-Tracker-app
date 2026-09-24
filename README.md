# QA Project Tracker

A single-file, offline web app for running a Quality Assurance improvement project. Built around the "TaskFlow Release Quality Improvement" example: reduce post-release defects by 30% within two release cycles.

## Getting Started

1. Download `qa_project_tracker.html`.
2. Double-click it to open in any modern browser (Chrome, Edge, Firefox, Safari).
3. No installation, server, or internet connection is needed.

## Features

| Tab | What it does |
|---|---|
| **Dashboard** | Four KPI cards (defect density, test coverage, critical bugs post-release, customer satisfaction) with progress bars toward target. Type a new value in a card to update it. |
| **Defects** | Log defects with a title, severity (1-5) and status (Open, In Progress, Closed). Change status or delete entries at any time. |
| **Checklist** | Preventive QA activities for the sprint (code review, CI tests, FMEA review, audits, requirements sign-off, smoke test). Tick items off as done. |
| **Risk Register** | FMEA-style table of potential failures, their effect, severity, and mitigation. |
| **PDCA** | Editable Plan / Do / Check / Act notes for the current sprint. Click **Save Notes** to store them. |

## How to Use It

1. Record your baseline KPI values on the **Dashboard**.
2. Each sprint, work through the **Checklist** and log any issues found in **Defects**.
3. Review the **Risk Register** when planning new features.
4. At the end of the sprint, update the KPIs and fill in the **PDCA** notes: what you planned, what you did, what the results showed, and what you will change next.
5. Repeat each sprint and compare KPI progress against the targets.

## Data and Privacy

- All data is stored in your browser's `localStorage`. Nothing is sent anywhere.
- Data is tied to the browser and the file location you opened it from. Opening the file in a different browser, or moving it to another folder, will show a fresh, empty tracker.
- Clearing your browser's site data will erase your entries.

## Customizing

Open the HTML file in a text editor and look near the bottom of the file, in the `<script>` section:

- `defaultKpis` — change KPI names, baselines, targets, and units.
- `defaultChecklist` — edit the checklist items.
- The Risk Register rows are plain HTML in the `tab-risk` section and can be edited directly.

To reset the tracker to its defaults, clear the site data for the page in your browser settings.

## Known Limitations

- Data is not shared between users or devices.
- No export/import of data yet. Copy important figures out manually.
- The Risk Register is read-only in the app; edit it in the HTML file.

## Related Concepts

- **QA vs QC:** QA prevents defects through process; QC finds defects in the product.
- **PDCA:** Plan-Do-Check-Act, the continuous improvement loop used each sprint.
- **FMEA:** Failure Mode and Effect Analysis, used to flag design risks early.
