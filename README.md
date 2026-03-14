# azure-intune-endpoint
This repository documents the design and implementation of a modern Microsoft Intune endpoint management. Itdemonstrates a cloud-native, identity-first endpoint lifecycle using Microsoft Entra ID and Microsoft Intune. 
It simulates real-world enterprise deployment workflows including device onboarding, configuration enforcement, compliance validation, and application deployment.

Documentation includes configuration steps, validation evidence, and troubleshooting scenarios to demonstrate practical administration skills.


Architecture Summary

This lab follows a modern endpoint lifecycle:

User Sign-In (Entra ID)
↓
Device Entra Join
↓
Intune Auto Enrollment
↓
Security Group Assignment
↓
Configuration Profile Deployment (Windows Hello for Business)
↓
Compliance Policy Evaluation
↓
Application Deployment (VLC Media Player)
↓
Device State = Compliant + Managed

Technology Stack
Microsoft Entra ID (Azure AD)
Microsoft Intune (Endpoint Manager)
Windows Hello for Business
Windows 11 Pro (Hyper-V VM)
Identity-driven endpoint management
Compliance and Configuration Profiles
Microsoft Store Application Deployment
Documentation Structure
The lab is organized according to lifecycle phases:

Phase	Description
Tenant Setup	Entra ID preparation and MDM configuration
Device Enrollment	Azure AD Join and Intune auto-enrollment
Configuration Profile	Windows Hello for Business enforcement
Compliance Policy	Device security validation
Application Deployment	Intune app deployment and verification
Skills Demonstrated
Identity-first endpoint management
Microsoft Entra ID device lifecycle
Intune configuration and compliance separation
Windows Hello for Business enforcement
Group-based deployment targeting
Endpoint troubleshooting and validation
Application deployment using Microsoft Intune
Lab Environment
Microsoft 365 Business Premium Trial Tenant
Microsoft Entra ID
Microsoft Intune (Endpoint Manager)
Windows 11 Virtual Machine (Hyper-V)
Key Design Concepts
Modern device management (MDM vs traditional GPO)
Cloud-native policy enforcement
Security baseline enforcement
Lifecycle-based deployment methodology
Outcome
Successfully built and validated a fully managed Windows endpoint demonstrating:

Azure AD device join
Automatic Intune enrollment
Configuration profile enforcement
Compliance validation
Application deployment
Endpoint operational verification
This lab demonstrates a modern cloud-native equivalent of traditional Active Directory + Group Policy workflows.
