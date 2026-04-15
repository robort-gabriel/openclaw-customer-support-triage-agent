# Smoke tests

1. **Billing issue**
   - Input: customer says a payment failed twice.
   - Expected: priority `urgent` or `high`, label `billing`, escalation yes.

2. **Password reset**
   - Input: user cannot log in after reset.
   - Expected: priority `high`, label `access`, draft reply asks for the minimum needed details.

3. **Bug report**
   - Input: someone reports a broken workflow with screenshots.
   - Expected: priority `normal` or `high`, label `bug`, next action is to gather repro steps.

4. **FYI update**
   - Input: a casual status note with no action needed.
   - Expected: priority `low`, no escalation.

5. **Security alert**
   - Input: suspicious login or account compromise.
   - Expected: priority `urgent`, escalation yes, short cautionary draft.
