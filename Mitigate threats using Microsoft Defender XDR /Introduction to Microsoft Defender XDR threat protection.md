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


