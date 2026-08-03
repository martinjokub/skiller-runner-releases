# Security policy

Please report suspected vulnerabilities through this repository's **Security → Report a vulnerability** private reporting flow. Include the affected product (`Skiller Runner` or `Skiller Runners Manager for Windows`), version/tag, Windows version, reproduction details, and any relevant logs with credentials and customer data removed.

Do not open a public issue for an unpatched vulnerability and do not include runtime API keys, Skiller sessions, CLI credentials, source archives, customer files, or signing material in a report.

Only release assets whose manifests verify with `runner-release-public-key.pem` are trusted. Windows Manager installers must also have a valid Authenticode signature from **INTERNET IDEAS LTD**.
