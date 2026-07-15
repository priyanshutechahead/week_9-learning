# introduction to production postmortem template
- production postmortem => often called an incident report or retro
- it is a structured way to document what went wrong after a system failure, why it happened and most importantly how to prevent it from happening again.
- It is a "blameless" process, meaning the focus is on fixing broken processes and technical gaps rather than finding someone to blame.

## The Core Components
- Executive Summary: A brief, high-level overview of the incident. What happened, how long it lasted, and who was affected?
- Impact: A clear description of the damage. Did users experience downtime, data loss, or slow performance? How many users were impacted?
- Timeline: A chronological list of key events. When was the problem detected? When was it acknowledged? When was the fix implemented?
- Root Cause Analysis (The "Why"): This is the heart of the report. It details the underlying technical or process reasons for the failure. Many teams use the "5 Whys" technique here to dig past the surface-level cause.
- Resolution: A summary of how the team brought the system back to normal.
- Lessons Learned: A reflection on what went well during the response and what could have been handled better (e.g., better communication or better monitoring alerts).
- Action Items (The "Fix"): A concrete list of tasks assigned to specific team members to ensure the same issue doesn't recur. These should be tracked like any other feature or bug.

## Why Use a Template?
- Using a consistent format makes it easier for teams to spot patterns over time. If you notice the same "root cause" appearing in multiple postmortems, it highlights a systemic issue in your architecture or workflow that needs a deeper investment to solve.
- Is there a specific type of incident you are currently documenting, or would you like a blank template you can copy and paste for your next report?
