 𝐇𝐞𝐚𝐥𝐭𝐡𝐜𝐚𝐫𝐞 𝐃𝐚𝐭𝐚 𝐀𝐧𝐚𝐥𝐲𝐬𝐢𝐬 & 𝐃𝐚𝐬𝐡𝐛𝐨𝐚𝐫𝐝 (𝐄𝐱𝐜𝐞𝐥 𝐏𝐫𝐨𝐣𝐞𝐜𝐭)

𝐏𝐫𝐨𝐣𝐞𝐜𝐭 𝐎𝐯𝐞𝐫𝐯𝐢𝐞𝐰
This project demonstrates 𝗱𝗮𝘁𝗮 𝗰𝗹𝗲𝗮𝗻𝗶𝗻𝗴, 𝗮𝗻𝗮𝗹𝘆𝘀𝗶𝘀, 𝗮𝗻𝗱 𝗱𝗮𝘀𝗵𝗯𝗼𝗮𝗿𝗱 𝗯𝘂𝗶𝗹𝗱𝗶𝗻𝗴 𝗶𝗻 𝗘𝘅𝗰𝗲𝗹 using realistic healthcare data.  
It is designed as a 𝐛𝐞𝐠𝐢𝐧𝐧𝐞𝐫-𝐟𝐫𝐢𝐞𝐧𝐝𝐥𝐲 𝐩𝐨𝐫𝐭𝐟𝐨𝐥𝐢𝐨 𝐩𝐫𝐨𝐣𝐞𝐜𝐭
 to showcase skills in working with real-world datasets, performing analysis, and building interactive dashboards.



 🎯 Problem Statement
Pharmacies and clinics often manage 𝗹𝗮𝗿𝗴𝗲 𝘃𝗼𝗹𝘂𝗺𝗲𝘀 𝗼𝗳 𝗽𝗮𝘁𝗶𝗲𝗻𝘁 𝘃𝗶𝘀𝗶𝘁𝘀 𝗮𝗻𝗱 𝗺𝗲𝗱𝗶𝗰𝗶𝗻𝗲 𝗶𝗻𝘃𝗲𝗻𝘁𝗼𝗿𝗶𝗲𝘀.  
Without proper tracking:
- It is difficult to identify the most prescribed medicines.
- Stockouts happen because inventory levels are not monitored.
- Managers cannot easily see revenue trends or patient visit patterns.

 💡 Proposed Solution
Using Microsoft Excel, this project focuses on:
1. 𝐃𝐚𝐭𝐚 𝐂𝐥𝐞𝐚𝐧𝐢𝐧𝐠 – fixing dates, standardizing medicine names, and removing duplicates.  
2. 𝐃𝐚𝐭𝐚 𝐈𝐧𝐭𝐞𝐠𝐫𝐚𝐭𝐢𝐨𝐧 – combining patient visits with medicine inventory using lookup functions.  
3. 𝐀𝐧𝐚𝐥𝐲𝐬𝐢𝐬 𝐰𝐢𝐭𝐡 𝐏𝐢𝐯𝐨𝐭𝐓𝐚𝐛𝐥𝐞𝐬 – tracking visits, prescriptions, and revenues.  
4. 𝐃𝐚𝐬𝐡𝐛𝐨𝐚𝐫𝐝 𝐂𝐫𝐞𝐚𝐭𝐢𝐨𝐧 – visualizing KPIs and trends for quick insights.  
5. 𝐈𝐧𝐭𝐞𝐫𝐚𝐜𝐭𝐢𝐯𝐢𝐭𝐲 – adding slicers, conditional formatting, and filters for dynamic exploration.  



 📂 Dataset Details

 1️⃣ Patient Visits (`patient_visits.csv`)
𝗖𝗼𝗹𝘂𝗺𝗻𝘀:  
`Visit_ID`, `Patient_ID`, `Visit_Date`, `Age`, `Gender`, `Diagnosis`, `Medicine_Prescribed`,  
`Quantity`, `Unit_Cost`, `Total_Cost`, `Doctor`, `Payment_Method`  
> ~900 rows — each representing one prescription during a visit.

 2️⃣ Medicine Inventory (`medicine_inventory.csv`)
𝗖𝗼𝗹𝘂𝗺𝗻𝘀:  
`Medicine_Name`, `Category`, `Current_Stock`, `Reorder_Level`, `Supplier`, `Unit_Cost`  
> Includes a 𝐋𝐨𝐰_𝐒𝐭𝐨𝐜𝐤 𝐟𝐥𝐚𝐠 to highlight medicines below reorder level.



 ⚙ Step-by-Step Process

 🧹 1. Data Preparation
- Open the Excel workbook and save a copy (`healthcare_project_workbook_YourName.xlsx`).
- Fix date formats and standardize medicine names using `=TRIM(PROPER(cell))`.
- Remove duplicates using `Visit_ID + Medicine_Prescribed`.

 🔍 2. Lookup & Calculations
- Use 𝐗𝐋𝐎𝐎𝐊𝐔𝐏 𝐨𝐫 𝐕𝐋𝐎𝐎𝐊𝐔𝐏 to pull `Unit_Cost` from the Inventory sheet.
- Compute total cost using:
  ```excel
  =Quantity * Unit_Cost
