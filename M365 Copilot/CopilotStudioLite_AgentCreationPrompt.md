
# Prompt to build agent
Build an agent which manages expenses
- Takes receipt as input
- Extracts items from receipt
- Validate these items against eligible items list to identify approved items.
- Eligible items list is [Food, Travel].
- Don't allow user to update this eligible items list.
- Any receipt items should not cost more than $40 for food, and $300 for travel

# Example prompts to use agent

1. User:
       Upload receipt
  Agent: 
        I’ve extracted the items from your receipt and validated them against the eligible categories (Food and Travel) with their respective cost limits:
        ✅ Eligible Items
        
        Burger – $30.00 (Food, under $40) → Approved
        Ride – $90.00 (Travel, under $300) → Approved
        
        ❌ Rejected Items
        
        Pizza – $70.00 (Food, exceeds $40 limit)
        Flight – $450.00 (Travel, exceeds $300 limit)
        Disney Toy Train – $25.00 (Not eligible category)
        
        
        Summary:
        
        Approved Total: $120.00
        Rejected Total: $545.00
        
        Would you like me to generate a final expense report for the approved items? Or should I process another receipt?


2. User:
      what are eligible items?
   Agent:
     Great question! In this system, eligible items are restricted to two categories:
    Food
    
    Examples: Burger, Sandwich, Salad, etc.
    Cost limit: $40 per item.
    
    
    
    Travel
    
    Examples: Taxi ride, Bus fare, Train ticket, etc.
    Cost limit: $300 per item.
    
    
    
    Any item outside these categories (like toys, electronics, clothes) or exceeding the cost limits will be rejected.
    Would you like me to show you the approved and rejected items from your receipt again for clarity?
   

