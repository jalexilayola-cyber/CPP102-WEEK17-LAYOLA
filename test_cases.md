
# Test Cases: Simulated Device Monitoring and Alert System

**Name:** Your Name  
**Student Number:** Your Student Number  
**Section:** 1CPE-B  
**Date Tested:** October 18, 2026

## Test Cases

I made these test cases to check if my program works correctly. I tested valid and invalid inputs to see if the program displays the correct results and handles mistakes properly.

| Test Case | Input or Action | Expected Result | Why I Expected This Output | Actual Result | Pass/Fail |
|---|---|---|---|---|---|
| TC01 | Select option 1 to view readings. | The program displays 28, 31, 35, 37, and 29. | These are the initial readings given in the project instructions. | The program displayed all five readings. | Pass |
| TC02 | Select option 2, enter 33, then select option 1. | The program accepts 33 and adds it to the readings. | The value is a whole number between 0 and 100. | The program accepted 33 and added it as the sixth reading. | Pass |
| TC03 | Select option 2 and press Enter without typing a value. | The program rejects the empty input. | A reading must contain a valid whole number. | Record the result after testing. | Pending |
| TC04 | Select option 2 and enter `abc`. | The program rejects the non-numeric input. | Only whole-number readings are allowed. | Record the result after testing. | Pending |
| TC05 | Select option 2 and enter `-1`. | The program rejects the reading. | Readings must be between 0 and 100. | Record the result after testing. | Pending |
| TC06 | Select option 2 and enter `101`. | The program rejects the reading. | Readings above 100 are outside the allowed range. | Record the result after testing. | Pending |
| TC07 | Select option 3 to classify readings. | 28 and 29 are NORMAL; 31 and 35 are WARNING; 37 is CRITICAL. | Classification depends on the temperature thresholds. | Record the result after testing. | Pending |
| TC08 | Select option 4 to generate the summary before adding readings. | The program displays 5 readings, total 160, average 32.00 °C, minimum 28 °C, maximum 37 °C, and the correct category percentages. Overall status is ATTENTION REQUIRED. | The summary must calculate statistics and classify all initial readings correctly. | Record the result after testing. | Pending |
| TC09 | Enter `8` at the main menu. | The program displays an invalid-choice message. | Menu choices must be from 1 to 5. | Record the result after testing. | Pending |
| TC10 | Select option 5 to exit. | The program displays a goodbye message and terminates. | Option 5 is the program's exit command. | Record the result after testing. | Pending |

## Conclusion

The test cases check the program's menu options, input validation, reading classifications, summary calculations, and exit function. The results will help determine whether the program meets the project requirements.