# Grade-Fetcher✔
![](useless/show.png)
## Tools I Used🛠
- The whole processing from **backend** to **frontend** is taken care by **[Python]**.
- **[Pyqt5]** offers a great frontend library for **Python**,and this is what i made my UI.
- Additionally i used **[Pyqt5]** designer tools for rapid development of UI.
- At backend **[Selenium]** web drivers runs and connect to my university website and fetch the required data.
- At same time the data gets saved to **Excel-file** using **[Openpyxl]** library.
## How To use🖱
![](useless/showgif.gif)
- Clone this repo and extract files to your desired location.
- Open **Grade-Fetcher->App->app.exe**.
- If you see a **Command Terminal**, its fine it acts as a error box.
- Any error while fetching data or internal code error will be show in **Command Terminal**.
- Main UI should just appear immediately.
- The whole UI is made very simple to understand and work on, but still you can refer this **[Video]** for your doubts.
## How It Works🤔
- Its very simple, just like connecting diffrent blocks in lego.
- So i created a UI that looks almost same as our university results **[Portal]**.
- As we can see one can easily get other student marks by simply entering the roll-no.
- **But what if the user wants to get all results of his classmate's and compare himself with others?**
- That's where my **Grade-Fetcher-App** come's to play.
- Insted of manually entering each roll-no my **Grade-Fetcher-App** will do that for you.
- User enters **Starting Roll-no** ,  **Ending Roll-no** , **Semester** and chooses the **Excel-File** to save the marks.
- **Grade-Fetcher-App** will check for **Validity** of all input's and progress of validation can be seen in the **Progress Bar**
- Once all the inputs are verified then **Pyqt5** send this data to **Selenium** web drivers.
- Now **Selenium** open a chrome window and connects to **[Portal]** and starts entering data into the text-field and clicks on **Get-Result** button automatically.
- Once result page is obtained it fetches **Student-Name**  , **Student-Roll-No** , **Student-GPA** , **Student-CGPA**.
- And passes this data to **[Openpyxl]** which saves data into user selected **Excel-File**.
- This process keeps on repeating until  **Ending Roll-no** is reached.
- After getting data for all the **Roll-no** the browser gets closed, which is indication that its safe to open the excel file and check the data that **Grade-Fetcher-App** got.
