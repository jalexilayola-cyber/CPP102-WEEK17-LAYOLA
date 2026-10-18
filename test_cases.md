# Test Cases: Simulated Device Monitoring and Alert System

**Name:** Layola, Jahzeel Alexi 
**Student Number:** 2601312 
**Section:** 1CPE-B  
**Date Tested:** October 18, 2026

## Test Results

| Test Case | Test Description | Test Input | Expected Result | Status |
|---|---|---|---|---|
| TC-01 | View initial readings | Select `1` | Displays 28, 31, 35, 37, and 29 °C | PASS* |
| TC-02 | Add a valid reading | Select `2`, enter `32` | Reading is added successfully | PASS* |
| TC-03 | Reject a negative reading | Select `2`, enter `-5` | Displays an invalid input message | PASS* |
| TC-04 | Reject a reading above 100 | Select `2`, enter `101` | Displays an invalid input message | PASS* |
| TC-05 | Reject nonnumeric input | Select `2`, enter `abc` | Displays an invalid input message | PASS* |
| TC-06 | Reject empty input | Select `2`, enter nothing | Displays an invalid input message | PASS* |
| TC-07 | Classify a normal reading | Enter or use `28` | Classified as NORMAL | PASS* |
| TC-08 | Classify the warning threshold | Enter or use `30` | Classified as WARNING | PASS* |
| TC-09 | Classify the upper warning threshold | Enter or use `35` | Classified as WARNING | PASS* |
| TC-10 | Classify a critical reading | Enter or use `37` | Classified as CRITICAL | PASS* |
| TC-11 | Generate the initial summary | Select `4` | Count: 5; total: 160; average: 32.00 °C; minimum: 28; maximum: 37 | PASS* |
| TC-12 | Verify classification percentages | Select `4` | NORMAL: 2 (40%); WARNING: 2 (40%); CRITICAL: 1 (20%) | PASS* |
| TC-13 | Verify overall system status | Select `4` | Displays ATTENTION REQUIRED | PASS* |
| TC-14 | Exit the program | Select `5` | Program terminates normally | PASS* |

\*Replace `PASS` with `NOT TESTED` until you have run and verified that test.

## Conclusion

The test cases cover the program's menu options, reading validation, temperature classification, summary calculations, alert status, and program termination. The system passes the tests when the actual output matches the expected results.