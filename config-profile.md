# Configuration Profile – Windows Hello for Business (Intune)

## Objective

Create and deploy a configuration profile using Microsoft Intune to enforce Windows Hello for Business authentication on managed Windows devices.

---

## Environment

Platform: Microsoft Intune  
Device: INTUNEWIN11_01 (Windows 11 Hyper-V VM)  
Profile Type: Settings Catalog  
Assignment: INTUNE-Test-Devices group  

---

## Configuration Steps

1. Navigated to:

Intune Admin Center → Devices → Configuration profiles → Create profile

2. Selected:

Platform: Windows 10 and later  
Profile Type: Settings Catalog

3. Configured Windows Hello for Business settings:

- Require PIN
- Enable WHfB authentication
- Enforce security policies

Screenshot:

![Configuration Profile Created](../screenshots/09-configuration-profile-success.png)

---

## Policy Assignment

The configuration profile was assigned to the INTUNE-Test-Devices group to trigger enforcement.

---

## Validation Evidence

Windows Hello enforcement workflow:

![PIN Setup Attempt](../screenshots/06-whfb-pin-setup-attempt.png)

![WHFB Policy Applied](../screenshots/10-whfb-policy-applied.png)

![WHFB PIN Enforcement](../screenshots/11-whfb-pin-policy-enforcement.png)

![PIN Successfully Configured](../screenshots/12-whfb-pin-configured-success.png)

---

## Troubleshooting Encountered

During initial PIN setup, Windows returned an error during provisioning.

Resolution:

- Forced Intune sync
- Restarted test VM
- Reattempted sign-in

PIN setup completed successfully after remediation.

---

## Outcome

Configuration profile successfully enforced Windows Hello for Business authentication and updated device authentication posture.
