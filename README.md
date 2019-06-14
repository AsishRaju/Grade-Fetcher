# Grade-Fetcher✔
![](useless/show.png)
## What It Does❓
- Gets complete Section (Class) results in one click without manually entering each student roll-no from **[Portal]**.
- With the help of easily understandable UI, user enters the mentioned details and clicks on **GET DATA** button.
- **Grade-Fetcher-App** then saves the data obtained in excel file. 
## Tools I Used🛠
- The whole processing from **backend** to **frontend** is taken care by **[Python]**.
- **[Pyqt5]** offers a great frontend library for **Python**,and this is what i used to make my UI.
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
- User enters **Starting Roll-no** ,  **Ending Roll-no** , **Semester** and chooses the **Excel-File-Location** to save the marks.
- **Grade-Fetcher-App** will check for **Validity** of all input's and progress of validation can be seen in the **Progress Bar**
- Once all the inputs are verified then **Pyqt5** send this data to **Selenium** web drivers.
- Now **Selenium** open a chrome window and connects to **[Portal]** and starts entering data into the text-field and clicks on **Get-Result** button automatically.
- Once result page is obtained it fetches **Student-Name**  , **Student-Roll-No** , **Student-GPA** , **Student-CGPA**.
- And passes this data to **[Openpyxl]** which saves data into user selected **Excel-File**.
- This process keeps on repeating until  **Ending Roll-no** is reached.
- After getting data for all the **Roll-no** the browser gets closed, which is indication that its safe to open the excel file and check the data that **Grade-Fetcher-App** got.
## Know Problems❌
- **Grade-Fetcher-App** dosen't respond when  **Selenium** browser is running.
- **Grade-Fetcher-App** dosen't work well with slow internet connection (<=5Mbps)
- **Grade-Fetcher-App-UI**  dosen't adapts itself when the window is resized.
- **A lot of code optimization is required which can make app perform better**
## Work In Progress🚧 
- Working on **Code optimization**.
- Adding feature to get the **Whole university result of a paticular department for a paticular Semester**.
- Adding feature to generate **Rank of the student based on their CGPA**.
- Working on a **RESPONSIVE UI**.
## How To Contribute🤝 
- Yes,it is open source you can clone and change code to your need.
- for any clarification on code or want to contribute contact vashish888@gmail.com or Dm me on [Instagram].

## Update-v1.0.1
- Added ability to fetch all the subject marks and also account for elective subjects;
- No need to fill excel file before hand for heading , my app will do it for you;

 ```bash
note-i compare myself with others as a competitive spirit which help me improve myself but not everyone thinks the same so don't think i treat other based on their grades.
Thank You.
```

[Video]: <https://youtu.be/zqiqtzCW5tM>
[Instagram]: <https://www.instagram.com/iamash1sh/>
[Python]: <https://www.python.org/>
[Pyqt5]: <https://pypi.org/project/PyQt5/>
[Selenium]: <https://www.seleniumhq.org/>
[Openpyxl]: <https://openpyxl.readthedocs.io/en/stable/#>
[Portal]: <https://doeresults.gitam.edu/onlineresults/pages/Newgrdcrdinput1.aspx>
