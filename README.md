ALGORITHM
Algorithm: Community Waste Reporting and Collection

Step 1: Start.
Step 2: Display the waste reporting menu.
Step 3: Enter the user's name.
Step 4: Enter the waste location.
Step 5: Enter the type of waste.
Step 6: Enter a description of the waste problem.
Step 7: Check whether all required information has been entered.
Step 8: If information is missing, display "Incomplete report" and request the information again.
Step 9: If the information is complete, save the report.
Step 10: Set the report status to "Pending".
Step 11: Assign the report to a collection worker.
Step 12: Change the status to "Assigned".
Step 13: Collection worker visits the reported location.
Step 14: Check whether the waste has been collected.
Step 15: If the waste has not been collected, keep the status as "Assigned".
Step 16: If the waste has been collected, change the status to "Collected".
Step 17: Close the report.
Step 18: Display the final status.
Step 19: End.

# PROG101-Assignment1-Rosemarie-Fredrica-Princess-John-905006208

PSEUDOCODE
BEGIN

DISPLAY "Community Waste Collection and Reporting System"

INPUT user_name
INPUT location
INPUT waste_type
INPUT description

IF user_name = EMPTY OR
   location = EMPTY OR
   waste_type = EMPTY OR
   description = EMPTY THEN

      DISPLAY "Incomplete report"
      DISPLAY "Please enter all required information"

ELSE

      SAVE report
      status = "Pending"

      DISPLAY "Report submitted successfully"

      ASSIGN report to collection_worker
      status = "Assigned"

      DISPLAY "Report assigned to collection worker"

      INPUT collection_completed

      IF collection_completed = YES THEN
            status = "Collected"
            DISPLAY "Waste collected successfully"

            status = "Closed"
            DISPLAY "Report closed"

      ELSE
            status = "Assigned"
            DISPLAY "Collection still pending"
      END IF

END IF

# PROG101-Assignment1-Rosemarie-Fredrica-Princess-John-905006208

