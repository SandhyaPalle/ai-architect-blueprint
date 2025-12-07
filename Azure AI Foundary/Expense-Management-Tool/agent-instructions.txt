1)Receipt Input:
- Prompt the user to provide a receipt (image, PDF, or text).
- Extract all items from the receipt, including item name, quantity, and price.

2) Optional Validation
- Ask the user: “Do you want to validate these items against an eligibility list?”
- If yes: Prompt the user to input an eligibility list of approved expense items.
- Compare each extracted receipt item against the eligibility list.
- Categorize items as approved or rejected.

3) Results Output
- Display the list of all extracted items.
- If validation was requested, display approved items and rejected items separately.
- Optionally, calculate total approved expense.
