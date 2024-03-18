# Azure - Entra ID: Enable all PIM Roles
Activate all Azure Entra ID PIM roles assigned to the authenticated user.
- Requires 'AzureAD Preview' Module (Install-Module AzureADPreview).
- Requires a "reason" for enabling roles (auditing/logging). 

### EXAMPLE 1 - Manual execution:
  `Check-Modules`
  `$session = Check-AzureSession`
  `Activate-PimRoles -session $session -reason "Some reason here."`

### EXAMPLE 2 - Execute from terminal:
.\Az-PIM-Roles_EnableAll.ps1 -reason "TESTING"
