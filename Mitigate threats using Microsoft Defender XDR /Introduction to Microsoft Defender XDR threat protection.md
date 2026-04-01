# Introduction 

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/934740df-86c0-45b0-b6f7-3f49a2f912e2" />

#

## Explore Extended Detection & Response (XDR) response use cases

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/bcff54b0-b8b9-4161-9ce7-bd26afa53ca8" />

#

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/64d16ff7-0a11-421d-813e-f7c071993103" />


#

## Understand Microsoft Defender XDR in a Security Operations Center (SOC)

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/16efb78e-f31a-45f5-849e-1e0052e23a21" />

#

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/467a31c6-25e1-4582-8a0d-f7207c0619ec" />

#

# 🧠 Microsoft Graph 

---

## 🎯 Imagine This...

Socho ek **super app** hai 📱  
jo sab jagah ka data ek hi jagah pe laata hai:

- Emails 📧  
- Files 📂  
- Users 👤  
- Devices 💻  
- Security alerts 🚨  

👉 Is super app ka naam hai: **Microsoft Graph**

---

## 🌐 Microsoft Graph Kya Hai?

👉 Ye ek **single door 🚪** hai  
jahan se tum Microsoft ke sab systems ka data dekh sakte ho

📌 Door ka address: https://graph.microsoft.com

---

## 🤔 Pehle Problem Kya Thi?

❌ Har service ka alag gate hota tha  
- Email alag  
- Files alag  
- Users alag  

👉 Confusing 😵

---

## ✅ Ab Kya Hai?

👉 Ek hi gate 🚪 = Microsoft Graph  
👉 Sab kuch ek jagah se access

---

## 📦 Microsoft Graph Kya-Kya Dekh Sakta Hai?

### 📧 Emails & Chat
- Outlook  
- Teams  

---

### 📂 Files
- OneDrive  
- SharePoint  

---

### 👤 Users & Security
- Microsoft Entra ID  
- Devices  
- Permissions  

---

### 💻 Devices
- Computers  
- Mobiles  

---

## 🔐 Microsoft Graph Security API (SUPER IMPORTANT 🔥)

👉 Ye ek **security helper robot 🤖** hai

---

## 🤖 Ye Robot Kya Karta Hai?

👉 Socho school me:
- 5 teachers alag-alag report dete hain 📄  

👉 Robot:
- Sab reports collect karta hai  
- Ek report bana ke deta hai 📊  

---

## 🧠 Real Life Me:

``` id="flow"
App → Graph Security API → Defender + Sentinel + Others → Result

```

# 

🎯 Ye Kaam Karta Hai:

✅ 1. Sab jagah se alerts laata hai

👉 Multiple tools → one place

# 

✅ 2. SIEM ko bhejta hai

👉 Example: Microsoft Sentinel

# 

✅ 3. Automatic action leta hai
Block ❌

Allow ✅

Alert 🚨

# 

✅ 4. Investigation me help karta hai

👉 Kaun? Kab? Kya? 🤔

#  

✅ 5. Smart banata hai system ko

👉 Data se learn karta hai

# 

✅ 6. SOC ka kaam easy karta hai

👉 Less manual work

---
# 🔍 Advanced Hunting (SOC Superpower 🔥)

👉 Detect bad activity using queries

## 🧠 Language Used:

👉 KQL (Kusto Query Language)

## 📌 Example4

``POST https://graph.microsoft.com/v1.0/security/runHuntingQuery``

``
{
 "Query": "DeviceProcessEvents 
 | where InitiatingProcessFileName =~ \"powershell.exe\" 
 | project Timestamp, FileName 
 | order by Timestamp desc 
 | limit 2"
}
``

🧠 **Ye Query Kya Karta Hai?**

👉 **Check karta hai:**

PowerShell kaha use hua

👉 Output:

Time ⏱️

File name 📄

<img width="2738" height="1487" alt="image" src="https://github.com/user-attachments/assets/b8d5fbf0-326a-4608-ba6c-e82e9b0d83aa" />

## 🛠️ Kaha Use Karte?

Graph Explorer

Microsoft Defender

---


<img width="1686" height="893" alt="image" src="https://github.com/user-attachments/assets/df17057d-dcf2-4008-ac38-030c0b89f156" />

# 

Azure Sentinel is a cloud-native (SIEM) solution that delivers intelligent security analytics across your entire organization. It collects data at cloud scale across all users, devices, applications, and infrastructure, on-premises and in multiple clouds. And it enables Security Operations teams to make threat detection, investigation, and response more efficient with Al and automation.

<img width="1701" height="934" alt="image" src="https://github.com/user-attachments/assets/fa4944c3-a2d0-4e54-bd6c-d8cde177e6dd" />

#

This is the Azure Sentinel Incidents page, which provides an overview of all incidents detected in your environment. In this example, you can see three incidents, which were created by Microsoft 365 Defender, Azure Sentinel, and Azure Defender, respectively.

Let's investigate the high severity alert titled "Potential malware uploaded to a storage blob container." To do so, select the incident title.

<img width="1699" height="913" alt="image" src="https://github.com/user-attachments/assets/fea36b80-670e-4df3-a2d3-ad74738f9701" />

#

To see if there is any immediate action that needs to be taken to protect the organization, we can investigate this alert in Azure Defender.

<img width="1693" height="858" alt="image" src="https://github.com/user-attachments/assets/d304496f-dad0-421a-8618-ce40ce0af411" />

#

Azure Defender helps protect your Azure and hybrid cloud workloads with built-in XDR capabilities. Customized threat intelligence and prioritized alerts allow you to focus on what matters the most.

Let's explore the entitie related to this alert.

<img width="1694" height="940" alt="image" src="https://github.com/user-attachments/assets/09fd88e4-0c29-4343-9f8a-7a0d24df68be" />

#
We can also see the name of the malware that was detected in the scanned file. Azure Defender was able to detect this file because it used a known bad hash.

Now let's see how we can use Azure Defender to take action.

<img width="1706" height="921" alt="image" src="https://github.com/user-attachments/assets/e57f012f-c9d9-4057-b846-f6943859ea65" />

#

<img width="1914" height="957" alt="image" src="https://github.com/user-attachments/assets/e365d9ce-90ab-4d66-afd0-852905ba5a94" />

#

<img width="1918" height="935" alt="image" src="https://github.com/user-attachments/assets/f3af60ed-fe05-4032-ace6-3ae11aed1349" />

#

<img width="1913" height="948" alt="image" src="https://github.com/user-attachments/assets/564598af-5955-44dd-9f67-1b1c215f7f3b" />


#

<img width="1918" height="926" alt="image" src="https://github.com/user-attachments/assets/c767e708-41ae-41e0-aa69-c75a61b146a1" />


#

<img width="1919" height="941" alt="image" src="https://github.com/user-attachments/assets/09aa1c52-c3fc-4a4b-a32f-3df1e5f70a12" />


#

<img width="1916" height="933" alt="image" src="https://github.com/user-attachments/assets/258200f2-65c0-49b0-993d-af24238440bf" />

#

<img width="1918" height="951" alt="image" src="https://github.com/user-attachments/assets/d7ebaa19-e17e-49e1-9fae-2a2ecb6c6df5" />


#

<img width="1917" height="935" alt="image" src="https://github.com/user-attachments/assets/9f75c3c3-b4ce-4570-87c2-3db1d1f24a29" />


#

<img width="1919" height="906" alt="image" src="https://github.com/user-attachments/assets/4e8faa17-fd79-4f85-ae7b-b60b1a5533ca" />


#

<img width="1919" height="554" alt="image" src="https://github.com/user-attachments/assets/713c13aa-ee52-4855-91b4-df3c11665386" />

#

<img width="1919" height="940" alt="image" src="https://github.com/user-attachments/assets/4e60a953-8d2d-47e4-afcd-e048c6e69460" />


#

<img width="1918" height="934" alt="image" src="https://github.com/user-attachments/assets/25511cf8-63c2-4510-a6b9-d39088159faf" />

#

<img width="1902" height="940" alt="image" src="https://github.com/user-attachments/assets/03ce34e3-f360-47e9-af2e-fddd5cb33ff3" />


#

<img width="1912" height="939" alt="image" src="https://github.com/user-attachments/assets/1c2ecdb3-98bd-4fe8-b73d-993b7280dedc" />


#

<img width="1909" height="947" alt="image" src="https://github.com/user-attachments/assets/22db45d0-6251-4537-8871-bbf524db5a34" />


#

<img width="1918" height="932" alt="image" src="https://github.com/user-attachments/assets/e77b20a3-43a5-4fe5-ac08-1ccf7142a974" />

#

<img width="1913" height="947" alt="image" src="https://github.com/user-attachments/assets/d9ae19fa-a8a5-40cc-a8ee-07c3755c3f91" />

#

<img width="1911" height="934" alt="image" src="https://github.com/user-attachments/assets/b847876b-8fc5-464c-99b2-255944504605" />


#

<img width="1915" height="961" alt="image" src="https://github.com/user-attachments/assets/91b8909d-bc6f-40bc-a736-cca6e9a6bff3" />


#

<img width="1917" height="947" alt="image" src="https://github.com/user-attachments/assets/9fb0e49c-d29d-477e-a7e6-5a2979397ad3" />


#

<img width="1909" height="925" alt="image" src="https://github.com/user-attachments/assets/1b365ef1-d49c-4c19-9686-499aeda49720" />

#

<img width="1919" height="955" alt="image" src="https://github.com/user-attachments/assets/99dcd0af-7551-4e60-a153-5f51647a998f" />

#

<img width="1917" height="964" alt="image" src="https://github.com/user-attachments/assets/2e056606-00d1-42b0-9799-5369aa2d6076" />

#

<img width="1919" height="674" alt="image" src="https://github.com/user-attachments/assets/dd0fdb29-9e43-436e-a7a4-af02af695093" />

#
<img width="1880" height="956" alt="image" src="https://github.com/user-attachments/assets/36fe0288-f169-4320-a2ed-10b93853b2f5" />

#

<img width="1913" height="953" alt="image" src="https://github.com/user-attachments/assets/9fc7d22e-8692-4d88-9ccd-3092593823b4" />

#

<img width="1906" height="933" alt="image" src="https://github.com/user-attachments/assets/064154a2-1500-4d18-a355-56d267475fcf" />

#



#

