# Telco-security-research

# Security Research & Vulnerability Disclosures

Public vulnerability research focused on telecommunications security, 4G/5G core networks, protocol fuzzing, and security vulnerability discovery.

This repository documents published CVEs, coordinated vulnerability disclosures, and security issues reported to open-source projects and technology vendors.

## Published CVEs

### Ella Core — 5G Core Network

| CVE | Description | Severity | Advisory |
|---|---|---|---|
| CVE-2026-32319 | AMF DoS via undersized integrity-protected NAS payload | High | [GHSA](https://github.com/advisories/GHSA-m9pm-w3gv-c68f) |
| CVE-2026-32320 | AMF DoS via malformed NGAP PathSwitchRequest | Moderate | [GHSA](https://github.com/advisories/GHSA-j478-p7vq-3347) |
| CVE-2026-33281 | Panic triggered by invalid PDU Session IDs | Moderate | [GHSA](https://github.com/advisories/GHSA-q669-4gmv-g8mf) |
| CVE-2026-33282 | Panic triggered by malformed NGAP Location Report | High | [GHSA](https://github.com/advisories/GHSA-826q-wrq4-p23x) |
| CVE-2026-33283 | Panic triggered by malformed ULNASTransport | Moderate | [GHSA](https://github.com/advisories/GHSA-3366-gw57-fcm5) |

**Research:** 5G AMF robustness, NGAP/NAS protocol fuzzing, input validation, and denial-of-service vulnerabilities.

### free5GC — 5G Core Network

| CVE | Description | Severity | References |
|---|---|---|---|
| CVE-2022-38870 | Unauthenticated disclosure of registered UE, subscriber, tenant and user information through the webconsole | High (NVD) | [NVD](https://nvd.nist.gov/vuln/detail/CVE-2022-38870) · [Original report #387](https://github.com/free5gc/free5gc/issues/387) |

**Research:** Authentication bypass, subscriber information disclosure, and 5G core management interface security.

### Ericsson Packet Core Controller (PCC)

| CVE | Description | Severity | References |
|---|---|---|---|
| CVE-2025-59180 | Hardcoded credentials in the alarm system enabling unauthorized access to alarm and alert information from within the cluster | Medium (CVSS 4.0) | [CVE](https://www.cve.org/CVERecord?id=CVE-2025-59180) · [Ericsson PSIRT](https://www.ericsson.com/en/about-us/security/psirt/security-bulletin-pcc-july-2026) |

**Attribution note:** The public Ericsson advisory credits other researchers/organizations. My individual contribution to this finding should be documented separately and confirmed before it is presented as an individually credited discovery.

## Public Security Vulnerability Reports

### Open5GS

| Issue | Finding | Original Report |
|---|---|---|
| #4341 | SMF crash caused by malformed Extended Protocol Configuration Options (EPCO) during PDU Session Establishment | [GitHub Issue #4341](https://github.com/open5gs/open5gs/issues/4341) |
| #4357 | MME crash caused by malformed S1AP/NAS Attach Request | [GitHub Issue #4357](https://github.com/open5gs/open5gs/issues/4357) |

### free5GC

| Issue | Finding | Original Report |
|---|---|---|
| #387 | Unauthenticated exposure of registered UEs, subscriber information, tenants and users via the webconsole (CVE-2022-38870) | [GitHub Issue #387](https://github.com/free5gc/free5gc/issues/387) |

## Research Focus

- **5G Core Security:** AMF, SMF, UPF, NRF, NAS and NGAP
- **4G/LTE Core Security:** MME, S1AP, GTP and EPC
- **Protocol Fuzzing:** NGAP, S1AP, X2AP, PFCP, GTP and NAS
- **Vulnerability Discovery:** Memory safety, denial of service, authentication bypass and information disclosure
- **Telecom Infrastructure Security:** Network functions, management interfaces, Kubernetes and cloud-native deployments
- **Coordinated Vulnerability Disclosure:** Reporting vulnerabilities to maintainers and vendors

## Research Attribution

This repository is a public index of published findings and does not reproduce proprietary engagement material, confidential vulnerability reports, or non-public proof-of-concept code.
