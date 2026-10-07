# Assessment Notes

## Summary

Fixed five high-value issues across the backend, SQL, API validation, pagination, and frontend error handling.

## Fixes

1. Fixed SQL AND/OR precedence so status filtering applies correctly.
2. Removed artificial Thread.sleep() API delay.
3. Added validation for invalid pagination values.
4. Added HTTP 400 handling for invalid task status values.
5. Fixed the React loading state when API requests fail.

## What I Did Not Change

I did not redesign the UI, upgrade dependencies, or make broader architectural changes because the assessment prioritizes focused, high-value fixes.

## Biggest Remaining Risk

The backend retrieves all matching records before applying pagination in Java. This could become a performance concern with a much larger dataset, but changing it would require a broader pagination refactor.

## AI / Tools Used

Used ChatGPT to help identify potential issues, reason about root causes, and plan verification steps. All fixes were implemented and tested locally using the provided application and browser/API testing.
