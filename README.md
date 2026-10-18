# Simulated Device Monitoring and Alert System

**Student Name:** Layola, Jahzeel Alexi
**Student Number:** 2601312
**Section:** 1CPE-B  
**Course:** CPP102

---

## 1. Project Description

The **Simulated Device Monitoring and Alert System** is a Python program that stores and monitors simulated device temperature readings. Users can view readings, add valid readings, classify temperatures, and generate a summary. The program also determines the overall monitoring status based on the classifications.

## 2. Project Objectives

- Apply Python variables, lists, selection statements, loops, and functions.
- View and add temperature readings.
- Validate readings and accept only whole numbers from `0` to `100`.
- Classify temperatures as NORMAL, WARNING, or CRITICAL.
- Calculate the total, average, minimum, maximum, category counts, percentages, and overall status.
- Practice testing, debugging, documentation, and version control.

## 3. Features

- View the initial temperature readings.
- Add valid temperature readings.
- Reject empty, non-numeric, decimal, negative, and above-100 inputs.
- Classify readings using the specified temperature limits.
- Generate a summary of the readings.
- Display the overall monitoring status.
- Repeat the menu until the user chooses to exit.
- Handle invalid menu choices without terminating the program.

## 4. Tools and Requirements

| Tool | Purpose |
|---|---|
| Python 3 | Runs the program |
| Visual Studio Code or another code editor | Writes and edits the source code |
| Terminal or command prompt | Executes the program |
| Git and GitHub | Tracks changes and hosts the project repository |

The program uses Python's built-in features and does not require external packages.

## 5. How to Run

1. Save the source code as `device_monitor.py`.
2. Open the project folder in a terminal.
3. Run the program using:

   ```bash
   python device_monitor.py
   ```

4. Select an option from the menu.
5. Follow the displayed instructions.
6. Select option `5` to exit.

## 6. Menu Options

| Option | Function |
|---|---|
| `1` | View Readings |
| `2` | Add Reading |
| `3` | Classify Readings |
| `4` | Generate Summary |
| `5` | Exit |

## 7. Temperature Classification Rules

| Temperature | Classification |
|---|---|
| Below 30 °C | `NORMAL` |
| 30 °C to 35 °C, inclusive | `WARNING` |
| Above 35 °C | `CRITICAL` |

> **Note:** These temperature limits are for classroom simulation only and are not real device-safety standards.

### Overall Monitoring Status

- **ATTENTION REQUIRED** — At least one CRITICAL reading exists.
- **MONITOR** — No CRITICAL readings exist, but at least one WARNING reading exists.
- **NORMAL** — No WARNING or CRITICAL readings exist.

## 8. Sample Summary for the Initial Readings

The program starts with these readings:

`[28, 31, 35, 37, 29]`

| Measurement | Result |
|---|---:|
| Number of readings | 5 |
| Total of readings | 160 |
| Average temperature | 32.00 °C |
| Minimum temperature | 28 °C |
| Maximum temperature | 37 °C |
| NORMAL | 2 (40.00%) |
| WARNING | 2 (40.00%) |
| CRITICAL | 1 (20.00%) |
| Overall Status | **ATTENTION REQUIRED** |

The overall status is **ATTENTION REQUIRED** because the reading `37 °C` is classified as CRITICAL.

## 9. Sample Program Output

The following is the expected summary output when the program uses the initial readings and option `4` is selected.

```text
MONITORING SUMMARY
------------------
Number of readings : 5
Total of readings : 160
Average temperature : 32.00 °C
Minimum temperature : 28 °C
Maximum temperature : 37 °C

NORMAL : 2 (40.00%)
WARNING : 2 (40.00%)
CRITICAL : 1 (20.00%)

Overall Status: ATTENTION REQUIRED
```

## 10. Testing

Use `test_cases.md` to document the test cases and their results. Tests should cover:

1. Viewing the initial readings.
2. Adding a valid reading.
3. Rejecting empty input.
4. Rejecting non-numeric input.
5. Rejecting readings below `0`.
6. Rejecting readings above `100`.
7. Checking temperature classifications, including the boundary values `30 °C` and `35 °C`.
8. Generating the summary.
9. Rejecting an invalid menu choice.
10. Exiting the program.

Record the actual result and mark each test as **Pass** or **Fail** only after performing it.

## 11. Known Limitations

- Readings are stored only while the program is running.
- Added readings are lost when the program closes.
- The system uses simulated readings and does not connect to a real device or temperature sensor.
- The temperature classification rules are intended for the classroom activity, not for real-world safety decisions.
- The program does not keep a permanent history of readings.

## 12. Reflection

The most challenging part of this project was combining the menu, input validation, classification rules, and summary calculations into one program. I learned that input validation helps prevent invalid values from being added to the readings list. Testing boundary values such as `30 °C` and `35 °C` also helped me understand conditional statements. In the future, I would improve the program by adding a way to save readings so they remain available after the program closes.

## 13. Project Files

| File | Description |
|---|---|
| `device_monitor.py` | Contains the Python source code |
| `README.md` | Describes the project and explains how to run it |
| `test_cases.md` | Records test cases, expected results, actual results, and pass/fail status |

## 14. Git and GitHub

Git and GitHub are used to track project changes and host the source code online. Meaningful commits should document development progress, such as creating the menu, adding reading operations, implementing classifications, calculating the summary, validating inputs, testing, and writing documentation.

Before submission, ensure all required files are committed and pushed to the GitHub repository.