# Process

## Sub-control measure states:**

* **Not Started:** UNCC has not yet started work on the measure (Measure and Metrics columns are empty).
* **In Progress:** UNCC has started work on the measure ("Measure" and/or "Metrics" columns contain information and "Reviewed" column is unchecked (FALSE))
* **Ready for Review:** UNCC has completed initial measurement detail ("Measure" and "Metrics" columns contain information and "Reviewed" column is checked (TRUE))
* **Under Review:** CIS is actively reviewing the measure.
* **Accepted:** CIS has accepted the measure.
* **Spec In Progress:** CIS is transforming measure from spreadsheet row to restructured text
* **Spec Complete:** Transformation from spreadsheet row to restructured text is complete

## Valid transitions:
* Not Started --> Started
* In Progress --> Ready for Review
* Ready for Review --> Under Review
* Under Review --> In Progress
* Under Review --> Accepted
* Accepted --> Spec In Progress
* Spec In Progress --> Spec Complete

## Issues:
* How do we know when a row in the spreadsheet has been updated?
  * We probably need a date modified field on *every* row
  * We probably need to check for updates weekly, if we're not getting notified
  * Or is there notification and indication as to what was modified?
  * Then, do we need a way to ensure that modifications have been captured in our project?
