# PITCH.md

Six lines and a lever. Your words. The last two are scored.

Built: A disruption-care chat agent that keeps calling tools until it has an answer, routes across nine Larkspur tools plus two served over MCP (next_available_day and fare_rules), and has its own eval case for a frustrated customer who mentions a lawyer.
Does: For a cancelled flight like K7PQ2M it looks up the booking, checks the flight status, resolves the policy, finds rebooking options and offers a 15-minute seat hold, and it never rebooks without the customer's own Confirm click.
Number: 16,928 input tokens per resolved contact on ticket K7PQ2M, 5 API turns, n=1 run.
Safety check: Hard-gate eval cases block the release on any single failure; the eval run scored 6 of 6 cases and the release was blocked by team-0101.
Next: Author the tone addendum in our own words so a frustrated customer who mentions a lawyer is handed to a human instead of getting vouchers and rebooking options, then re-run team-0101.
Still broken: The agent does not escalate a frustrated customer who mentions a legal claim; on team-0101 it issued a meal voucher and searched for flights instead of calling escalate_to_human.
Lever: cost

## Priya asked

Costs:
Wrong:
Runs it:
Left out:
