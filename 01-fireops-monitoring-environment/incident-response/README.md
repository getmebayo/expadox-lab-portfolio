# Incident-Response Playbooks

## SSH brute-force attack

### Identification

- Confirm repeated failed SSH authentication attempts.
- Identify the source IP and targeted account.
- Determine whether any authentication attempt succeeded.

### Containment

Preferred options:

1. Fail2Ban or automated temporary banning
2. SSH rate limiting
3. Restricting SSH to trusted networks
4. Firewall blocking for confirmed malicious sources

### Eradication

- Rotate exposed credentials.
- Disable unnecessary password authentication.
- Remove unauthorised accounts.
- Review SSH configuration.
- Disable direct root login.

### Recovery

- Confirm approved administrators retain access.
- Review active sessions.
- Monitor authentication logs.
- Maintain heightened monitoring.

## Network reconnaissance

### Identification

- Review Suricata alerts.
- Identify source and destination systems.
- Determine scan scope and intensity.

### Containment

- Apply rate limiting.
- Block confirmed malicious scanners.
- Disable unnecessary services.
- Close unnecessary ports.

### Recovery

- Verify required services remain available.
- Confirm monitoring remains operational.
- Continue watching for follow-up exploitation attempts.

## Privilege escalation

### Identification

- Review sudo activity.
- Identify affected users and commands.
- Check for active elevated sessions.

### Containment

- Terminate unauthorised privileged processes.
- Revoke unnecessary sudo access.
- Suspend confirmed compromised accounts.

### Recovery

- Restore only approved privileges.
- Validate system integrity.
- Continue enhanced monitoring.
