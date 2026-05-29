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

![image alt](https://github.com/Hamedadams01/Active-Directory/blob/4dc6520f6c06cc8ff3cc61a57698b85238104ea5/Screenshot_2026-03-11_111012.webp)

 From here I needed to install the Active Directory Domain Services role by clicking "Add roles and features"

![image alt](https://github.com/Hamedadams01/Active-Directory/blob/4dc6520f6c06cc8ff3cc61a57698b85238104ea5/Screenshot_2026-03-11_125509.webp)

I selected Active Directory Domain Services (AD DS) and added required features. This installed the tools needed to create and manage a domain.

![image alt](https://github.com/Hamedadams01/Active-Directory/blob/4dc6520f6c06cc8ff3cc61a57698b85238104ea5/Screenshot_2026-03-11_125533.webp)

Now I selected ‘Add a new forest’ and named my domain `houtech.locl`. The system automatically created a NetBIOS name, which came out as HOUTECH
![image alt](https://github.com/Hamedadams01/Active-Directory/blob/4dc6520f6c06cc8ff3cc61a57698b85238104ea5/Screenshot_2026-03-11_125836.webp)

I selected “Add a new forest” and named my domain houtech.locl . Below that it’s showing my NetBIOS name came out as HOUTECH

![image alt](https://github.com/Hamedadams01/Active-Directory/blob/4dc6520f6c06cc8ff3cc61a57698b85238104ea5/Screenshot_2026-03-11_130008.webp)

The install is done. Server Manager now shows AD DS and DNS are both running. This confirms the server is officially a domain controller.

![image alt](https://github.com/Hamedadams01/Active-Directory/blob/4dc6520f6c06cc8ff3cc61a57698b85238104ea5/Screenshot_2026-03-11_131015.webp)
