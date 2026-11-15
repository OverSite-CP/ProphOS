# Change log

What changed in ProphOS, newest first, in plain words. Each release on the
[Releases](../../releases) page carries the same notes and the installer's SHA-256 checksum.

Version numbers: **1.0.0** is the first public release. Before it, ProphOS was tried by a small
group of pilot users on numbered test builds (**0.0.x**, the number rising with every build);
those are summarised below by month.

---

## 1.0.0 (December 2026)

The first public release, on the Microsoft Store. A signed installer for direct download
follows.

### One app, and a free trial

- **One app.** Anyone can open, view, print and export XER programmes without an account.
  Sign in with a Microsoft account to edit; what you can do is set by your plan.
- **Launch trial.** Sign in during the first three months after launch and get six months of
  ProphOS Team free. A card says **Your Team trial has started** and when it ends. No card is
  asked for and nothing is charged when it ends; you then choose a plan or carry on free, with
  every file kept and read-only.
- **Microsoft Store edition.** The Store keeps ProphOS up to date; the app's own update check
  is switched off in the Store edition.

### Make a programme, and build its WBS

- **Create programme.** Start a new programme in a project, blank or from another programme as a
  template (its calendars, codes, user fields, resources with rates, options and currency, as you
  tick them; never its activities). A step-by-step window asks for the Project ID, title, dates,
  calendars, codes and a starter WBS, then shows an **export readiness** check of what an XER file needs
  before the programme is made. It is in **Setup**, **Integrate**, the start screen and the
  right-click menu of a project.
- **WBS editing in the grid.** Add a child or sibling, rename, indent, outdent, move up or down,
  delete (move the contents up, or delete the node with its activities) and **Move to WBS…**,
  from the Plan tab's WBS group or a WBS row's right-click menu. Drag activities onto a node, or
  a node into another, and see where it will land before you let go. **Build WBS…** shows the
  whole tree in one window. Every change is one undo step, and works the same in a shared
  programme and a branch.
- **Link the selected activities** with **Ctrl+L**, right-click › **Add link**, or
  **Plan › Logic › Link**. Activities are linked in the order you clicked them, finish-to-start;
  links that would make a loop, or that touch a WBS row, are refused with a reason.

### Open and save XER files

- **Multi-project XER import.** A file holding several projects opens on an import screen that
  sorts them into main programmes and their baselines. You confirm each one's role.
- **An XER inside a .zip.** Open, Add programme, Clean on import and dropping a file on the window
  all take a .zip; with several XER files inside, you choose one. The zip is not changed.
- **Clean on import.** Leave out what you do not want in the programme as it comes in: unused
  calendars, resources, activity code values and user fields, costs, expenses, or odd characters.
  Presets and tick boxes, with a preview that counts what goes and checks the dates are unchanged.
- **Clean on export.** The same for the file you send: **Full**, **Send to client**, **No costs**,
  **Logic only** or **Anonymise**. The programme keeps everything; only the file is cleaned.
- **Baseline in an XER export.** **Save as XER…** can include one of the programme's baselines
  (off by default), written as a project of its own for you to make a baseline.
- **XER export with nothing else installed.** ProphOS writes XER itself, with no Java.

### Tables and the Activity panel

- **Export table to Excel.** Send the activity table, the rows you chose, or the rows shown after
  your filters, to a workbook with the table's columns, real Excel dates and the WBS as Excel
  groups. A preview and a format window set the title, colours, columns and page.
- **All the dates in the relationship tables.** Predecessors and successors can show early start
  and finish, late start and finish, and actual start and finish.
- **Activity panel tables.** Relationships and resources are tables like the main grid: choose the
  columns, type a lag or units in the cell, change a type or resource from a drop-down, and show
  predecessors and successors stacked or side by side.
- **Show these in the table.** From a schedule health finding, show only the activities it
  flags. With **Show only traced** and **Zoom to traced** on the Analyse tab, a **Filtered by**
  chip says what is hiding the rest and clears it.
- **A tidier ribbon.** The Plan, Analyse and Layouts tabs now fit a 1366 x 768 screen at 100%:
  less-used commands sit under **Edit › More** or in compact pairs, and Layouts has **Rows** and
  **View** groups. Nothing was removed.

### Comments, people and your account

- **Closing comments.** Closing a comment needs a note saying how it was resolved, shown at the
  end of the thread. A closed comment is reopened with a reason. Only the comment's author, its
  assignee or an administrator can close or reopen it, and the author and assignee get a notice.
  The comment sheet and its Excel export carry who closed it and the closing comment.
- **Names.** People are shown by their Microsoft display name in changes, comments, notices and
  **Also here**. Your Windows account and PC names are not used when you are signed in.
- **Delete my account.** **Administer › My account › Delete my account…** deletes your account
  yourself, after listing what goes and what stays.
- **Reports are your choice.** An issue or crash report names your workspace, project and
  programme only if you tick the box, and shows you exactly what will be sent first.

### Forecasts and the rest

- **Insights learns from your own programmes.** Forecast duration and Slip risk are learnt on
  your PC from the open programme's earlier updates (and, if you choose, the project's other
  programmes). Nothing is sent anywhere to make a forecast.

### Fixed

- Integrate review and Compare: the action buttons are one size and line up on the right.
- Narrow and scaled screens: the chart stays visible, and one focus ring and one button order
  (Close or Cancel first, the main action last at the right) are used throughout.

---

## Pilot builds (private testing)

### November 2026 (0.0.931 to 0.0.996)

- **Insights tab** (new): Forecast duration, with its likely range, and Slip risk, with a
  watch-list and **Why?** to show the main reasons behind each forecast.
- **POAP:** track several activities in one item; **Show build-up** adds pages listing the
  activities behind each item (PDF, PowerPoint and Excel); drawn links can be reshaped by
  dragging their joints, with **Reset route** to undo it.
- **Save as XER:** optionally include a baseline.
- **Open a multi-project XER** through the new import screen.
- **XER export** no longer needs Java on the PC.
- **Command line:** ProphOS can start with `--find=<text>` to open on a search.
- Fixed: selecting a row in a branch you had just opened sometimes did not show its details.

### October 2026, second half (0.0.703 to 0.0.923)

- **Accounts and roles:** sign in with a Microsoft account from the account chip (top right);
  **Administer › Accounts and access** for My account, Members and roles, Activity and audit,
  and Policies. Roles: owner, administrator, planner, reviewer and viewer.
- **Branches:** make a what-if copy of a programme, compare it with main, and integrate it back
  by accepting or rejecting each change.
- **Micro plans:** plan one activity in detail, see the roll-up, and **Use** its duration for
  scheduling or **Embed** it permanently. Micro plans follow the activity's status.
- **POAPs and dashboards** can be drawn from a branch, with **Main (current)** as the baseline.
- **Change report** (**Report › Evaluate change…**): what moved between two versions, with
  graphs, checks and tables, exported to PDF and Excel.
- **Comments** on activities, a **comment sheet**, and saved **custom filters** shared in the
  project.
- **Right-click menus** on the activity table and column titles.
- **Undo by change** on shared programmes; edits made while another is applying are queued, not
  lost.
- **Large programmes:** faster opening, reviewing and comparing; tested at about 98,000
  activities.
- **Crash log and crash report:** **Administer › Help › Show log folder** and **Send crash
  report…**, which shows you exactly what will be sent first.
- **One copy at a time:** starting ProphOS again brings the open copy to the front.
- **Name:** the app took the name ProphOS. Settings from earlier test builds are carried across
  on first start.
- Fixed: Compare failed on resources without rates; a false "closed unexpectedly" message;
  a lost edit when many edits arrived at once; a crash on reloading a branch.

### October 2026, first half (0.0.359 to 0.0.695)

- **Editing** (first pilot builds): add, delete, copy, cut, paste, fill down, replace, renumber,
  dissolve, Build WBS, constraints, progress, undo and redo, and Schedule (F9).
- **Setup:** company, project and programme details, calendars, activity codes and user fields;
  **Push** to bring programmes in line with the project's calendars, codes and resources.
- **Resource & Cost:** resources, assignments and expenses, read from and written back to XER.
- **Workspaces and the Navigator:** regions, clients, projects and programmes, on this PC or in
  Microsoft 365; several workspaces at once; **Remove from list**.
- **Working together:** several people in one programme at once, with notices, a Changes panel
  and an Activity ID clash dialog. **F5** brings in everyone's changes.
- **Baselines and versions:** capture, assign and upload baselines; baseline bars (project
  baseline and BL1 to BL3) on the Gantt; keep and revert versions.
- **Layouts:** five built-in layouts and your own; panels, bars, timescale, grouping, sorting by
  any column, outline levels and columns, exported as `.prpl` files.
- **Analyse:** trace logic backward and forward by levels, driving path, multiple float paths,
  look-ahead and filters.
- **Dashboards:** a pop-out window of charts over live data: S-curves, histograms, milestone
  tracker, earned value for reporting, with templates.
- **POAP** (plan on a page): swimlanes and items tied to activities, frozen versions, and export.
- **Schedule health:** the DCMA 14-point check, with a project's own thresholds.
- **XER compliance** (Administer): ProphOS's dates against the dates stored in the file.
- **Report an issue** (Administer) and **Updates…** (check automatically, or Check now).
- **Unsaved changes** are asked about before closing, quitting or signing out; **Ctrl+W** closes
  the programme.
- **Print / PDF:** vector sheets from A4 to A0.

### September and early October 2026 (before the pilot)

- The scheduling engine: forward and backward passes, the XER schedule options, calendars,
  constraints, level-of-effort and WBS-summary activities, progress and out-of-sequence work,
  measured against the dates stored in real XER programmes until it agreed.
- The first read-only viewer: open an XER, see it scheduled, the Activity details panel, and
  trace to the cause of any difference from the stored dates.
