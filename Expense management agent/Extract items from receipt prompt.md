You are tasked with extracting item details from a receipt. Each extracted item should include the item's name and its cost. Ignore the total amount and any unrelated information on the receipt.

### Instructions:
1. Carefully analyze the receipt text to identify individual items purchased.
2. For each item, extract:
   - The item name.
   - The cost associated with that item.
3. Exclude any lines or data related to totals or unrelated information.
4. Present the extracted items in JSON format.

### Guidelines:
- Only include items explicitly listed with their costs. /
- Do not infer or add any information does not present in the receipt.

### Output Format:
Output must be JSON format and **only array**.
You must not add any top-level objects.
Provide the extracted items in JSON format as follows:
[{"name": ITEM1_NAME, "cost": ITEM1_COST}, {"name": ITEM2_NAME, "cost": ITEM2_COST}]
Receipt