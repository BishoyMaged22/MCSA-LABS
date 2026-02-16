# Local Administrator Accounts on Domain-Joined Machines

When a Windows 10 machine is joined to a domain, permissions are typically controlled by domain policies.  
However, it is still important to maintain a **local administrator account** on the machine.

## Why Local Admin Is Needed

- **Emergency Access**  
  If the domain controller is unavailable (network outage, replication issues, or domain corruption), local admin credentials allow access to the machine.

- **Troubleshooting**  
  Local admin rights are required to perform certain diagnostic or recovery tasks, such as fixing drivers, repairing OS components, or accessing safe mode.

- **Security & Control**  
  Domain admins may have elevated rights, but a local admin ensures there is always a fallback account that is independent of domain authentication.

- **Separation of Roles**  
  Regular domain users remain standard users on the machine, while domain admins are granted admin rights.  
  The local admin account provides an additional layer of control outside domain policies.

## Best Practice

- Keep at least one **local administrator account** enabled and secured with a strong password.  
- Use domain accounts for daily administration, but rely on the local admin for recovery scenarios.  
- Document the local admin credentials securely (e.g., password vault).

---
##lab
- manage
<img width="341" height="321" alt="image" src="https://github.com/user-attachments/assets/ccae3e56-1801-4877-a7c3-30e86110d710" />
- those are the admins in this machine
<img width="1919" height="570" alt="image" src="https://github.com/user-attachments/assets/6c56a29a-8db1-445c-b8d0-2d58843a0387" />
- for adding new local admin i need Domain permission
  <img width="1919" height="576" alt="image" src="https://github.com/user-attachments/assets/d40443da-75f6-43f9-b66f-23076a7a9866" />
<img width="1919" height="568" alt="image" src="https://github.com/user-attachments/assets/1dfb3c3b-3c8e-46b2-9df1-0d4bb7c787ce" />
