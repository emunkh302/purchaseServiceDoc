# Express-O Demo Script


## Preparation checklist

- [ ] **Present features:** Each team member has at least one feature to show and
  a 2–3 minute speaking slot.
- [ ] **Demo script:** Speaker names, feature order, and handoffs are filled in
  below.
- [ ] **Practice:** The full team has completed at least one practice run and
  updated this script to address timing or demo issues.

## Suggested speaker and feature order

The flow starts with the shop's catalog, then follows a customer through a sale
and finishes with the team's results.

| Order | Speaker | Feature | Target time |
|---|---|---|---:|
| Welcome | **[Presenter / facilitator]** | Introduce the team and Express-O | 1 minute |
| 1 | **Seydou** | Ingredients and drink recipes | 2–3 minutes |
| 2 | **Anthony** | Baked goods | 2–3 minutes |
| 3 | **Mike** | Recording a purchase and updating the customer account | 2–3 minutes |
| 4 | **Anthony** | Customer experience or another completed feature | 2–3 minutes |
| Close | **[Presenter / facilitator]** | Thank the audience and invite questions | 1 minute |

Adjust the order and remove unused rows to match the team's completed features.
Keep each member's segment focused on their own contribution.

## Opening — facilitator

“Hello, everyone. We’re **Team II**, and this is Express-O, a proof-of-concept
application for a local coffee shop. It helps the shop manage its menu, customers,
and purchases. We’ll walk through the shop experience from setting up products
to recording a sale.”

## Feature handoffs and talking points

### 1. Ingredients and drink recipes — Seydou

- Show a drink and its recipe.
- Explain the shop uses ingredients to make its drinks.
- If ready, show how ingredient availability affects whether a drink can be sold.

**Handoff:** “Now that we’ve seen how a drink is made, **Anthony** will show
what customers can choose alongside it.”

### 2. Baked goods — Anthony

- Show a baked good available for resale.
- Explain that baked goods come from a vendor and are offered to customers by the
  shop.

**Handoff:** “We have the products ready. **Mike** will show how a customer’s
purchase is recorded.”

### 3. Purchase recording — Mike

**Feature:** A drink purchase creates or reuses a customer account, records the
sale, updates lifetime spending, and deducts the drink's ingredients from stock.

**Demo steps:**

1. Start with a drink whose recipe uses an ingredient with visible stock.
2. Purchase the drink for a first-time customer using a demo name and email.
3. Show the recorded purchase and its total.
4. Show the customer's lifetime spending and the reduced ingredient stock.
5. If time permits, make a second purchase for the same email and show that the
   existing customer is reused and their lifetime spending increases.

**Speaker notes (2–3 minutes):**

“I worked on the purchase models, purchase repository, purchase service, related
validators, and purchase-service tests. I also reviewed teammates' branches to
help catch issues and keep features working together. A purchase line identifies
whether the item is a drink or baked good, which item it refers to, its quantity,
and the price recorded for the sale. The purchase itself keeps its customer,
timestamp, items, total, and repository-assigned ID.

I’ll record a drink purchase. The service checks that the drink and customer
references are valid, uses the current item price to calculate the total, and
records the purchase. For this drink, the recipe also uses stock, so the
ingredient amount goes down. The customer's lifetime spending goes up by the
purchase total. If this customer comes back, the shop can find the existing
account using the email rather than creating another one.”

**Handoff:** “That’s the purchase flow I worked on. **Anthony and Seydou** will show
**another completed feature**.”

### 4. Seydou — another completed feature

- Show one completed feature you worked on.
- Explain the customer or shop benefit in plain language.

**Handoff to close:** “That’s **another completed feature**. I’ll pass it back to **[facilitator]**
to wrap up.”

## Closing — facilitator

“That concludes our Express-O demo. Thank you for your time. We’re happy to answer
any questions.”

## Practice run

Schedule at least one practice run with the full team. Read the script aloud and
perform the demo steps in order.

- [ ] Confirm each speaker's name, feature, and handoff.
- [ ] Time each feature segment; keep it between 2 and 3 minutes per team member.
- [ ] Confirm the demo data, application, and purchase flow are ready before
  starting.
- [ ] Practice the full presentation from opening through questions.
- [ ] Note any confusing transitions, errors, or delays and update this script.
- [ ] Run through the updated presentation once more if the practice exposed
  issues that need another check.
