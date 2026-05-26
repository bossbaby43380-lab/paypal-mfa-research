# Observations

## OBS-001

### Observation
Multiple alternate HTTPS listeners expose similar TLS certificate chains associated with api.paypal.com.

### Evidence
- 443
- 8443
- 2053
- 2083

### Interpretation
Potential shared edge infrastructure.

### Security Relevance
May become relevant if authentication behavior differs across listeners.

### Status
Unverified