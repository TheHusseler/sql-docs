---
title: "SQL Server Login Password Strength"
description: "SQL Server Login Password Strength"
author: VanMSFT
ms.author: vanto
ms.date: "03/14/2017"
ms.service: sql
ms.subservice: security
ms.topic: conceptual
helpviewer_keywords:
  - "Best Practices [Database Engine]"
---
# SQL Server Login Password Strength
 [!INCLUDE [SQL Server](../../includes/applies-to-version/sqlserver.md)]
  This rule checks whether "Enforce password policy" of each [!INCLUDE[ssNoVersion](../../includes/ssnoversion-md.md)] login is enabled. If [!INCLUDE[ssNoVersion](../../includes/ssnoversion-md.md)] Authentication is enabled and if the operating system version is earlier than [!INCLUDE[winserver2003](../../includes/winserver2003-md.md)], an attacker could repeatedly exploit a known [!INCLUDE[ssNoVersion](../../includes/ssnoversion-md.md)] login password.  
  
## Best Practices Recommendations  
 We recommend that you upgrade the operating system to [!INCLUDE[winserver2003](../../includes/winserver2003-md.md)].  
  
 If [!INCLUDE[ssNoVersion](../../includes/ssnoversion-md.md)] Authentication is not required in your environment, use Windows Authentication.  
  
 Enable "Enforce password policy" for all the [!INCLUDE[ssNoVersion](../../includes/ssnoversion-md.md)] logins. Use [ALTER LOGIN](../../t-sql/statements/alter-login-transact-sql.md) to configure the password policy for the [!INCLUDE[ssNoVersion](../../includes/ssnoversion-md.md)] login.  
  
## For More Information  
 [Password Policy](../../relational-databases/security/password-policy.md)  
  
## See Also  
 [Monitor and Enforce Best Practices by Using Policy-Based Management](../../relational-databases/policy-based-management/monitor-and-enforce-best-practices-by-using-policy-based-management.md)  
  
  
