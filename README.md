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
| Password Recovery <br/>密碼復原 (SSPR)               | Self-Service Password Reset  |
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
* Registered password recovery authentication methods using a non-administrator test account <br/>and verified the registration status in Microsoft Entra Security info.<br/>
使用非管理員測試帳號註冊密碼復原驗證方式，並於 Microsoft Entra Security info 確認註冊狀態
<br />
<br />
<b>Task 7: Test Self-Service Password Reset<br/> (測試自助式密碼重設)</b><br/>
<img src="https://i.imgur.com/3aZhNjz.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
* Successfully completed Self-Service Password Reset using a non-administrator test account <br/>and verified that account access could be restored with the new password.<br/>
使用非管理員測試帳號成功完成自助式密碼重設，並驗證可透過新密碼恢復帳號存取<br/>
<br />
<br />
<b>Task 8: Review Password Reset Audit Logs<br/> (檢查密碼重設稽核紀錄)</b><br/>
<img src="https://i.imgur.com/DRi94xz.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
* Reviewed Microsoft Entra audit logs and verified the successful self-service password reset event<br/> to demonstrate visibility into password recovery activities.<br/>
檢查 Microsoft Entra 稽核紀錄，確認自助式密碼重設成功事件，<br/>以展示密碼復原活動的可視性與稽核能力<br/>
<br />
<br />

---------

<h2>Results｜專題結論</h2>

This project demonstrated password security and recovery management in Microsoft Entra ID by combining password protection controls with Self-Service Password Reset (SSPR). Smart Lockout and a custom banned password list were configured to reduce the risks associated with repeated password-guessing attempts and predictable organisation-related passwords.

本專題透過整合密碼保護控制與自助式密碼重設 (SSPR)，實作 Microsoft Entra ID 中的密碼安全與復原管理。藉由設定 Smart Lockout 與自訂禁止密碼清單，降低重複密碼猜測及使用容易預測的組織相關密碼所帶來的風險。

SSPR was deployed to a selected group with defined authentication, registration, and notification requirements. The project extended beyond administrative configuration by validating password protection and password recovery from a user perspective, demonstrating how registered authentication methods can support secure account recovery without direct administrator intervention.

SSPR 以指定群組方式部署，並設定身分驗證、註冊及通知要求。本專題進一步從使用者角度驗證密碼保護與帳號復原流程，展示如何透過已註冊的驗證方式，在無需管理員直接介入的情況下安全恢復帳號存取。

Microsoft Entra audit logs were also reviewed to provide visibility into password recovery activities, connecting policy configuration, user validation, and administrative monitoring within a single identity security workflow.

最後透過 Microsoft Entra 稽核紀錄檢查密碼復原活動，將政策設定、使用者驗證與管理端監控整合為完整的身分安全工作流程。

<br />
<br />



---------

<h2>Security Insight｜安全洞察</h2>


Password security requires multiple complementary controls rather than relying on password complexity alone. Smart Lockout helps reduce repeated password-guessing attempts, while banned password policies restrict predictable terms that may otherwise satisfy basic password requirements. Together, these controls strengthen password-based authentication at both the sign-in and password creation stages.

密碼安全需要多種互補控制，而不能只依賴密碼複雜度。Smart Lockout 有助於降低重複密碼猜測行為，而禁止密碼政策則限制即使符合基本密碼要求、但仍容易被預測的詞彙。兩者結合後，可分別從登入與密碼建立階段強化密碼式驗證的安全性。

SSPR introduces an important balance between security and usability. Allowing users to recover their own accounts can reduce administrative workload and improve availability, but its security depends on properly scoped deployment, reliable authentication methods, and the protection of registered recovery information. Enabling SSPR for a selected group provides a controlled way to validate these settings before broader deployment.

SSPR 則呈現安全性與可用性之間的重要平衡。允許使用者自行恢復帳號可以降低管理負擔並提升可用性，但其安全性仍取決於適當的部署範圍、可靠的身分驗證方式，以及已註冊復原資訊的保護。先針對指定群組啟用 SSPR，可在擴大部署前以受控方式驗證相關設定。

Password recovery should also remain auditable. Self-service capabilities reduce direct administrator involvement but do not remove the need for visibility and accountability. Reviewing Microsoft Entra audit logs allows administrators to trace password reset activities and provides evidence that can support troubleshooting, governance, and security investigations.

密碼復原流程同樣必須具備可稽核性。自助式功能雖然減少管理員直接介入，但不代表可以放棄可視性與責任追蹤。透過 Microsoft Entra 稽核紀錄，管理員仍可追查密碼重設活動，並為故障排除、治理與安全事件調查提供可驗證的紀錄。

The Smart Lockout values used in this project were based on the lab requirements and should not be treated as universal production settings. In a real environment, password protection, lockout thresholds, recovery methods, and notification policies should be adjusted according to organisational risk, user requirements, and operational impact.

本專題使用的 Smart Lockout 參數依據實驗要求設定，不應視為所有正式環境皆適用的標準值。在實際組織環境中，密碼保護、鎖定閾值、復原方式及通知政策仍應依據組織風險、使用者需求與營運影響進行調整。


<br />
<br />

---------

<h2>Reference｜參考</h2>

* [Microsoft] [Microsoft Certified: Identity and Access Administrator Associate (SC-300)](https://learn.microsoft.com/en-us/credentials/certifications/identity-and-access-administrator/?practice-assessment-type=certification)<br/>
* [Microsoft] [Get started with identity and access labs](https://learn.microsoft.com/en-au/training/modules/get-started-identity-access-labs/)<br/>
<br/>
