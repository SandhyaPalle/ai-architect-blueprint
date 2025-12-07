1. Parse the JSON. 
2. Compare each item name against the eligible category of items. Eligible items are food, travel. Reject item above $300.
3. Return list of items with name, cost and eligibility which is either "approved" or "declined". You must not add any other status. Do not add anything besides JSON.
4. Write message with JSON only. Do not add any reasoning and explanation.


### Output formatReturn array only JSON. Do not add anything beside the provided schema.

[{"item": {"itemName": NAME, "cost":  COST}, "status": "approved", "reason": REASON_OF_STATUS}, {"item": {"itemName": NAME, "cost": COST}, "status": "declined", "reason": REASON_OF_STATUS}]
