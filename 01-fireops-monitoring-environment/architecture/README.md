# FireOps Monitoring Architecture

The FireOps monitoring environment uses a layered architecture:

1. Log sources generate endpoint, authentication, network and cloud events.
2. Wazuh agents collect and forward endpoint and server logs.
3. Suricata inspects network traffic and generates IDS alerts.
4. Wazuh Manager decodes events and applies built-in and custom rules.
5. OpenSearch stores and indexes security telemetry.
6. Wazuh Dashboard provides analysis, visualisation and alert investigation.
7. Response procedures guide containment, eradication and recovery.

See the project documentation in `../docs/` for the original architecture diagram and implementation evidence.
