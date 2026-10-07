# Microsoft Entra ID Password Security and Self-Service Password Reset

Microsoft Entra ID 密碼安全與自助式密碼重設 (SSPR)

<br/>

---------

<h2>Outline｜專題簡介</h2>

This project demonstrates password security management in Microsoft Entra ID, including password protection policies, Smart Lockout, custom banned passwords, and Self-Service Password Reset (SSPR).

本專題展示 Microsoft Entra ID 中的密碼安全管理操作，包括密碼保護政策、Smart Lockout、自訂禁止密碼清單，以及自助式密碼重設(SSPR)。

This explores how password protection policies can help prevent the use of weak or commonly used passwords, while SSPR enables users to securely recover access to their accounts through configured authentication methods.

本文探索如何透過密碼保護政策降低使用弱密碼或常見密碼的風險，同時透過 SSPR 讓使用者使用預先設定的驗證方式，安全地恢復帳號存取權限。

It also includes practical validation of password protection and password reset operations, followed by reviewing Microsoft Entra audit logs to verify the results and improve visibility into identity management activities.

亦包含密碼保護與密碼重設功能的實際驗證，並透過 Microsoft Entra 稽核紀錄檢查操作結果，以提升身分管理活動的可視性。

<br/>

---------

<h2>Key Learning Outcomes｜主要學習成果</h2>

* Configure Microsoft Entra password protection policies<br/>
設定 Microsoft Entra 密碼保護政策

* Configure Smart Lockout to reduce password-based attack risks<br/>
設定 Smart Lockout，以降低密碼型攻擊風險

* Create and enforce a custom banned password list<br/>
建立並啟用自訂禁止密碼清單

* Configure Self-Service Password Reset (SSPR) for a selected group<br/>
為指定群組設定自助式密碼重設 (SSPR)

* Configure SSPR authentication methods and registration requirements<br/>
設定 SSPR 驗證方式與註冊要求

* Configure password reset notifications<br/>
設定密碼重設通知

* Validate password protection and self-service password reset<br/>
驗證密碼保護與自助式密碼重設功能

* Review password reset activities through Microsoft Entra audit logs<br/>
透過 Microsoft Entra 稽核紀錄檢查密碼重設活動

* Understand how password protection and SSPR support secure identity lifecycle management<br/>
理解密碼保護與 SSPR 如何支援安全的身分生命週期管理

<br/>

---------

<h2>Tools and Concepts Covered｜涵蓋工具與概念</h2>

| Category 分類                                      | Tools / Concepts 工具 / 概念       |
| ------------------------------------------------ | ------------------------------ |
| Cloud Identity Management <br/>雲端身分管理          | Microsoft Entra ID |
| Identity Administration <br/>身分管理                | Microsoft Entra Admin Center |
| Premium Identity Features <br/>進階身分安全功能       | Microsoft Entra ID P2 (Trial) |
| Password Security <br/>密碼安全                     | Password Protection |
| Account Lockout <br/>帳號鎖定機制                    | Smart Lockout |
| Password Restrictions <br/>密碼限制                 | Custom Banned Password List |
| Password Recovery <br/>密碼復原                     | Self-Service Password Reset (SSPR) |
| Group-Based Configuration <br/>群組式設定            | Selected Group |
| Authentication Methods <br/>身分驗證方式              | Email, Mobile Phone, Mobile App Code |
| User Registration <br/>使用者註冊                    | SSPR Registration |
| Security Notifications <br/>安全通知                | Password Reset Notifications |
| Security Validation <br/>安全功能驗證                | Password Protection and SSPR Testing |
| Auditing and Monitoring <br/>稽核與監控              | Microsoft Entra Audit Logs |


<br/>

---------

<h2>Materials and Methods｜材料與方法</h2>

[Environment]

* Microsoft Azure Portal (Azure 雲端管理平台)</b>
* Microsoft Entra ID tenant (Entra ID 租戶環境)</b>
* Microsoft Entra ID P2 - Trial (Microsoft Entra ID P2 - 試用版)</b>
* Microsoft Entra admin center (Microsoft Entra 管理中心)</b>
* Microsoft 365 admin center (Microsoft 365 管理中心)</b>

[Tasks]

* Configure Password Protection (設定密碼保護政策)
* Validate Password Protection (驗證密碼保護政策)
* Enable SSPR for a Group (為群組啟用 SSPR)
* Configure SSPR Authentication Methods (設定 SSPR 驗證方式)
* Configure SSPR Registration and Notifications (設定 SSPR 註冊與通知)
* Register Password Reset Methods (註冊密碼重設驗證方式)
* Test Self-Service Password Reset (測試自助式密碼重設)
* Review Password Reset Audit Logs (檢查密碼重設稽核紀錄)
<br/>

---------

<h2>Practice｜實踐</h2> <p align="center">

<p align="center">
<b>Task 1: Configure Password Protection<br/> (設定密碼保護政策)</b><br/>
<img src="https://i.imgur.com/9fc7EYm.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
* Configured Smart Lockout to mitigate password-guessing attacks.<br/>
配置智慧鎖定功能以減輕密碼猜測攻擊<br/>
* Enable the custom banned password list (corresponding to a fictional company's name, location, and <br/>flagship product, respectively) to restrict the use of easily guessable, organization-related terms.<br/>
啟用自訂停用密碼清單（分別對應於虛構的公司名稱、地點和旗艦產品），<br/>以限制使用容易猜測的、與組織相關的術語<br/>
<br />
<br />
<b>Task 2: Validate Password Protection<br/> (驗證密碼保護政策)</b><br/>
<img src="https://i.imgur.com/v4w10mu.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
* Tested the custom banned password policy using a non-administrator account and <br/>verified that a restricted test password was rejected.<br/>
使用非管理員測試帳號測試自訂禁止密碼政策，並確認受限制的測試密碼遭到拒絕<br/>
<br />
<br />
<b>Task 3: Enable SSPR for a Group<br/> (為群組啟用 SSPR)</b><br/>
<img src="https://i.imgur.com/hWFb6Jn.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
* Enabled SSPR for the Project23 group to demonstrate controlled deployment of password recovery capabilities.<br/>
為 Project23 群組啟用自助式密碼重設 (SSPR)，以示範密碼復原功能的受控部署<br/>
<br />
<br />
<b>Task 4-1: Setting the Number of Authentication Methods<br/> (設定身份驗證方法的數量)</b><br/>
<img src="https://i.imgur.com/l3vdmmE.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b>Task 4-2: Configure the Authentication Method Policies<br/> (配置身份驗證方法策略)</b><br/>
<img src="https://i.imgur.com/hr6XF6W.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b>Task 5-1: Configure SSPR Registration<br/> (設定 SSPR 註冊)</b><br/>
<img src="https://i.imgur.com/V5hgOG4.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b>Task 5-2: Configure SSPR Notifications<br/> (設定 SSPR 通知)</b><br/>
<img src="https://i.imgur.com/hp4CRBo.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b>Task 6: Register Password Reset Methods<br/> (註冊密碼重設驗證方式)</b><br/>
<img src="https://i.imgur.com/hfFivIl.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
* Assigned Microsoft Entra ID P2 to the Project23 Microsoft 365 group through Microsoft Graph and <br/>verified the group-based license assignment in the Microsoft 365 Admin Center.<br/>
透過 Microsoft Graph 將 Microsoft Entra ID P2 指派給 Project23 Microsoft 365 群組，<br/>並於 Microsoft 365 Admin Center 驗證群組式授權結果<br/>
<br />
<br />
<b>Task 7: Test Self-Service Password Reset<br/> (測試自助式密碼重設)</b><br/>
<img src="https://i.imgur.com/3aZhNjz.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
* Assigned Microsoft Entra ID P2 to the Project23 Microsoft 365 group through Microsoft Graph and <br/>verified the group-based license assignment in the Microsoft 365 Admin Center.<br/>
透過 Microsoft Graph 將 Microsoft Entra ID P2 指派給 Project23 Microsoft 365 群組，<br/>並於 Microsoft 365 Admin Center 驗證群組式授權結果<br/>
<br />
<br />
<b>Task 8: Review Password Reset Audit Logs<br/> (檢查密碼重設稽核紀錄)</b><br/>
<img src="https://i.imgur.com/DRi94xz.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
* Assigned Microsoft Entra ID P2 to the Project23 Microsoft 365 group through Microsoft Graph and <br/>verified the group-based license assignment in the Microsoft 365 Admin Center.<br/>
透過 Microsoft Graph 將 Microsoft Entra ID P2 指派給 Project23 Microsoft 365 群組，<br/>並於 Microsoft 365 Admin Center 驗證群組式授權結果<br/>
<br />
<br />

---------

<h2>Results｜專題結論</h2>

This project demonstrated the administration of users, Microsoft 365 groups, group membership, and license provisioning within a Microsoft Entra environment. By using the Project23 group as a centralized management object, administrative tasks could be applied consistently at the group level rather than managed separately for individual users.

本專題實作 Microsoft Entra 環境中的使用者、Microsoft 365 群組、群組成員及授權配置管理。透過 Project23 群組作為集中式管理物件，可將管理作業一致地套用至群組，而非逐一管理個別使用者。

We also involved troubleshooting differences between Microsoft Entra tenants and limitations in the current Microsoft 365 Admin Center interface. Microsoft Graph was used to verify group properties and complete the Microsoft Entra ID P2 group-based license assignment, with the result subsequently validated through the Microsoft 365 Admin Center.

我們也檢視了 Microsoft Entra 租用戶之間的差異以及目前 Microsoft 365 管理中心介面存在的限制。透過 Microsoft Graph 驗證群組屬性並完成 Microsoft Entra ID P2 群組式授權指派，最後再回到 Microsoft 365 Admin Center 驗證實際結果。

<br />
<br />



---------

<h2>Security Insight｜安全洞察</h2>


Group-based identity and license management improves consistency, scalability, and auditability by associating access and service entitlements with managed groups instead of relying on repeated manual changes to individual accounts. This approach can reduce configuration errors and support more structured user lifecycle and access governance processes.

基於群組的身份和許可證管理透過將存取權限和服務授權與受管群組關聯，而非依賴對單一帳戶的重複手動更改，從而提高了一致性、可擴展性和可稽核能力。這種方法可以減少配置錯誤，並支援更結構化的使用者生命週期和存取治理流程。

The troubleshooting process also demonstrated that administrative roles, tenant boundaries, object properties, and application permissions are separate security controls. Holding the Global Administrator role does not automatically grant an application such as Microsoft Graph Explorer every API permission, while users, groups, licenses, and roles remain isolated between different Microsoft Entra tenants. Understanding these boundaries is important when diagnosing IAM issues and applying least-privilege administration.

本次故障排除亦呈現出管理角色、Tenant 邊界、物件屬性與應用程式權限屬於不同的安全控制層級。即使帳號具備 Global Administrator 角色，也不代表 Microsoft Graph Explorer 自動擁有所有 API 權限；不同 Microsoft Entra Tenant 之間的使用者、群組、授權與角色亦彼此隔離。理解這些安全邊界，是進行 IAM 問題診斷及落實最小權限管理的重要基礎。


<br />
<br />

---------

<h2>Reference｜參考</h2>

* [Microsoft] [Microsoft Certified: Identity and Access Administrator Associate (SC-300)](https://learn.microsoft.com/en-us/credentials/certifications/identity-and-access-administrator/?practice-assessment-type=certification)<br/>
* [Microsoft] [Get started with identity and access labs](https://learn.microsoft.com/en-au/training/modules/get-started-identity-access-labs/)<br/>
<br/>
