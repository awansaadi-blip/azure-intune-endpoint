# Compliance Policy – Windows 11 (Intune)

## Objective

Create and validate a compliance policy to enforce device security standards.

---

## Environment

Platform: Microsoft Intune  
Device: INTUNEWIN11_01  
Policy Type: Windows 10 and later Compliance Policy  

---

## Configuration Steps

Compliance policy created requiring:

- Secure Boot enabled
- Windows Hello PIN configured
- Device marked compliant

![Configuration Profile Success](../screenshots/09-configuration-profile-success.png)

---

## Policy Assignment

Assigned to INTUNE-Test-Devices group for staged validation.

---

## Validation Evidence

![WHFB PIN Configured](../screenshots/12-whfb-pin-configured-success.png)

![Device Compliance View](../screenshots/13-device-compliance-view.png)

![Device Compliance Success](../screenshots/14-device-compliance-success.png)

---

## Troubleshooting Encountered

Initial WHfB provisioning required manual sync before compliance evaluated correctly.

---

## Outcome

Device successfully transitioned to compliant state after configuration enforcement.
