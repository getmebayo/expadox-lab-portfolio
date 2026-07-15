# Detection Rule Catalogue

## Rule 1 — SSH brute force

**Data source:** `/var/log/auth.log`

**Detection condition:** Multiple failed SSH authentication attempts from the same source within a short period.

**Security objective:** Detect password guessing and credential-stuffing activity.

**Expected response:**

1. Identify the source IP.
2. Confirm whether authentication succeeded.
3. Review the targeted account.
4. Apply rate limiting or temporary blocking.
5. Rotate credentials if compromise is suspected.

## Rule 2 — After-hours login

**Data source:** Authentication and system logs.

**Detection condition:** Successful or failed login activity outside approved operating hours.

**Security objective:** Detect unusual account use or compromised credentials.

## Rule 3 — Privileged command execution

**Data source:** Syslog, authentication logs and sudo logs.

**Detection condition:** Use of `sudo`, root shells or privileged commands.

**Security objective:** Identify unauthorised administration and privilege escalation.
