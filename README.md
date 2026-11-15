# ProphOS

**Construction planning for XER programmes, on your own Windows PC.**

ProphOS opens XER files, reschedules them with its own engine, and gives planners the tools
to edit, review, compare and report on a programme without a separate scheduling database. Your programmes stay
on your computer, your network drive or your own Microsoft 365.

ProphOS is made by [OVERSITE PTE. LTD.](https://oversitecp.com), Singapore.

This repository holds ProphOS's public **releases**, the **[user guide (wiki)](../../wiki)** and
the **[issue tracker](../../issues)** for bug reports and ideas. The application's source code is
not published here.

---

## Contents

- [Key features](#key-features)
- [Get ProphOS](#get-prophos)
- [System requirements](#system-requirements)
- [Launch trial](#launch-trial)
- [Screenshots](#screenshots)
- [Help and support](#help-and-support)
- [Privacy and terms](#privacy-and-terms)

## Key features

- **Opens XER files** and schedules them with ProphOS's own engine, a critical path scheduling engine (F9) for XER programmes.
  A file of several projects is sorted into main programmes and their baselines for you.
- **Saves back to XER**, with resources, assignments, expenses, activity codes and user
  fields, and optionally one baseline.
- **Edit the programme** in a table and Gantt chart: add, delete, link (Ctrl+L), copy and paste,
  fill down, renumber, dissolve, build the WBS, update progress and reschedule (F9). Every change
  can be undone, even after scheduling.
- **Workspaces** arranged as workspace › region › project › programme, on this PC, a network
  drive or Microsoft 365 (SharePoint, Teams or OneDrive).
- **Work together** on one programme at the same time, with changes merged and clear notices
  when two people touch the same thing.
- **Branches** for what-if work, reviewed change by change before you integrate them back, and
  **micro plans** to plan one activity in detail.
- **Baselines and versions**: capture, assign and compare, with baseline bars on the Gantt.
- **Analyse**: trace logic, driving paths, multiple float paths, look-ahead, and a DCMA
  14-point **schedule health** check.
- **Insights**: forecast durations and slip risk, learnt on your PC from your own programmes'
  earlier updates. Nothing leaves your computer to make a forecast.
- **Report**: print to PDF from A4 to A0, live dashboards, plan-on-a-page (POAP) charts, and a
  change report between two versions, exported to PDF, PowerPoint or Excel.
- **Comments** on activities, a comment sheet, and a change log of who changed what.

See the [user guide](../../wiki) for each one.

## Get ProphOS

| Where | What you get | Updates |
|:--|:--|:--|
| **Microsoft Store** | Coming in December 2026 | By the Store |
| **Signed download** | `ProphOS-Setup-<version>.exe` from the [Releases](../../releases) page or OverSite's download page, signed by OVERSITE PTE. LTD., with its SHA-256 checksum | ProphOS checks and updates itself (an IT administrator can turn this off) |

Both are the same app. Install one, not both. To check a downloaded installer, compare its
checksum with the one on the release:

```powershell
Get-FileHash .\ProphOS-Setup-<version>.exe -Algorithm SHA256
```

See [Getting started](../../wiki/Getting-Started) for the first run.

## System requirements

- Windows 10 (version 1809 or later) or Windows 11, 64-bit.
- No Java, Python or .NET to install: everything ProphOS needs is inside the app.
- An internet connection to sign in, to get updates and to use Microsoft 365 workspaces.
  Opening and viewing a file needs no connection.
- A Microsoft account (work, school or personal) to edit. Opening, viewing, printing and
  exporting need no account.
- macOS and Linux are not supported yet.

## Launch trial

Sign in with a Microsoft account in the first three months after launch and get **six months of
ProphOS Team free**: no card needed, and nothing is charged when it ends. See
[Plans and licences](../../wiki/Plans-and-Licences).

## Screenshots

*Screenshots to follow. They are taken from invented demonstration programmes only.*

1. The main window: Plan tab, activity table and Gantt chart.
2. The Navigator with a workspace, regions, projects and programmes.
3. Opening a multi-project XER: main programmes and baselines.
4. Trace logic and float paths on the Analyse tab.
5. Insights: forecast duration and slip risk with "Why?".
6. A branch's integrate review.
7. A POAP (plan on a page).
8. A dashboard.
9. The change report.
10. Schedule health (DCMA 14-point).

## Help and support

- **User guide:** the [wiki](../../wiki).
- **Something wrong, or an idea?** Search the [issues](../../issues), then open a new one with
  the bug report or feature request form. You can also report from inside ProphOS:
  **Administer › Report an issue…**.
- **Questions by email:** [support@oversitecp.com](mailto:support@oversitecp.com).
- **Security issues:** please do not open a public issue. See [SECURITY.md](.github/SECURITY.md).

Please never attach a programme that holds confidential information to a public issue.

## Privacy and terms

- Privacy notice: [oversitecp.com, ProphOS › Privacy](https://oversitecp.com/#prophos/privacy)
- Terms of use: [oversitecp.com, ProphOS › Terms](https://oversitecp.com/#prophos/terms)
- What stays on your PC: [Privacy and data](../../wiki/Privacy-and-Data)

---

ProphOS is proprietary software, © OVERSITE PTE. LTD.. The documentation in this repository and its
wiki is licensed under [CC BY 4.0](LICENSE.md); the application is not.
Microsoft, Windows and Microsoft 365 are trademarks of the Microsoft group of companies.

OVERSITE PTE. LTD. · UEN 202551198K · 10 Sims Drive, #18-32, Singapore 387390
