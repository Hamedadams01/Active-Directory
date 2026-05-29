# Active Directory & Domain

**Overview**

---

In this home lab, I demonstrate the process of configuring an Active Directory Domain environment using Windows Server 2022. This includes promoting the server to a Domain Controller, configuring DNS, and establishing a fully functional domain.

This lab simulates a real-world enterprise setup where centralized identity and resource management is critical.

---

## **Objectives**

- Install Active Directory Domain Services (AD DS)
- Promote a server to a Domain Controller
- Configure a new domain
- Validate DNS functionality
- Verify domain services are operational

I’m back in Server Manager. I need to add the Active Directory role so this server can become a domain controller.

![Screenshot 2026-03-11 111012.png](attachment:7c46f59d-404a-4843-aded-5268e13a16ec:Screenshot_2026-03-11_111012.png)

 From here I needed to install the Active Directory Domain Services role by clicking "Add roles and features"

![Screenshot 2026-03-11 125509.png](attachment:aa998eb4-8d43-4b72-9273-e654055cfe4e:Screenshot_2026-03-11_125509.png)

I selected Active Directory Domain Services (AD DS) and added required features. This installed the tools needed to create and manage a domain.

![Screenshot 2026-03-11 125533.png](attachment:c321632d-d6b9-47e7-bddb-5dbf698c48ab:Screenshot_2026-03-11_125533.png)

Now I selected ‘Add a new forest’ and named my domain `houtech.locl`. The system automatically created a NetBIOS name, which came out as HOUTECH

![Screenshot 2026-03-11 125836.png](attachment:14d8b4ac-0884-480e-a262-b00177d66cce:Screenshot_2026-03-11_125836.png)

I selected “Add a new forest” and named my domain houtech.locl . Below that it’s showing my NetBIOS name came out as HOUTECH

![Screenshot 2026-03-11 130008.png](attachment:9a631764-000f-440e-b8d9-b9591fa5b948:Screenshot_2026-03-11_130008.png)

The install is done. Server Manager now shows AD DS and DNS are both running. This confirms the server is officially a domain controller.

![Screenshot 2026-03-11 131015.png](attachment:72f50ddd-e32f-45df-acaf-06f0f2df5a1d:Screenshot_2026-03-11_131015.png)
