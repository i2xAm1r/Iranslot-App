using System;
using System.Windows.Forms;

namespace CarGame
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
            timer1.Interval = 50; // سرعت حرکت ماشین
            timer1.Enabled = false;

            // اتصال ایونت‌های ماوس به فرم
            this.MouseDown += Form1_MouseDown;
            this.MouseUp += Form1_MouseUp;
        }

        private void timer1_Tick(object sender, EventArgs e)
        {
            // حرکت ماشین به سمت راست
            picCar.Left += 5;
        }

        private void Form1_MouseDown(object sender, MouseEventArgs e)
        {
            timer1.Enabled = true;
        }

        private void Form1_MouseUp(object sender, MouseEventArgs e)
        {
            timer1.Enabled = false;

            // بررسی برخورد با مانع (کله‌قندی)
            if (picCar.Right > picBarrier.Left && picCar.Left < picBarrier.Right)
            {
                MessageBox.Show("آفرین، برنده شدی!");
            }
            else
            {
                MessageBox.Show("متأسفانه، بازنده شدی!");
            }
        }
    }
}

## 🌟 About the Project
![image](https://github.com/user-attachments/assets/e1112814-615f-4c83-b9d0-101a83076b70)

<b>1. This is a Python project under Windows for faster testing of laptops in the company to help the expert advance in the repair process.<b><br>
<b>2. More features may be added in the future and the source code of this project is private<b>

## ⚆_⚆ About This [Iranslot](https://iranslot.com)
![image](https://github.com/user-attachments/assets/a731ccbe-e8f3-4758-b848-78b2003f4c05)


<b>[Iranslot](https://www.iranslot.com) is a complete set of services in providing the best IT services in Iran and the most equipped specialized clinics for repairs, training and parts supply<b><br>



---
### 🎯 Features

**Software:**
- **Full Test CPU**: Stresses the CPU so you can check health and usage percentage.
- **System Information**: It shows you all the information from 0 to 100 of your system.
- **HDD SSD Info**: This feature shows you all the information about the size, model, and serial number of the hard drive or SSD.
- **Check URL**: In this feature, you can enter your desired URL and click check to test the link against the available DNS servers in the program and notify you.
- **Lcd Test**: This feature allows you to test and inspect the LCD screen with the color of your choice to find out if there are any dead pixels, lines, or black spots.
- **Battery Test**: This feature provides a laptop battery test report that includes the battery health, serial number, and number of times it has been charged, and automatically shows you
- **DNS capability**: In the DNS Changer section, you can select the DNS you want and click on apply dns to apply it. If you want to delete the DNS, click on clear dns.
- **Report PDF**: It saves the device information for you and outputs a PDF, and also has the ability to print.
- **System Monitor**: monitoring that shows the percentage of RAM and CPU usage in real time.
- **Speed Test**: Ability to test internet speed online with report
- **Browser**: A simple in-app browser
## Supported DNS Servers

By default, the app comes with a list of popular DNS servers in Iran.

| DNS Server   | IP Addresses          |
| ------------ | ---------------------|
| Shecan DNS   | 178.22.122.100,185.51.200.2 |
| Begzar DNS   | 185.55.225.25,185.55.226.26 |
| 403 DNS      | 10.202.10.202,10.202.10.102 |
| Radar DNS    | 10.202.10.10,10.202.10.11 |
| Electro DNS  | 78.157.42.100,78.157.42.101 |
## 👀 ScreenShot
![image](https://github.com/user-attachments/assets/a9d40fc2-a7c2-4af0-9a37-4f226a871981)


## :handshake: Contact

2xAm1r - [Telegram](https://t.me/bftup) - Awmircode@gmail.com

Project Link: [https://github.com/i2xAm1r/Iranslot-App](https://github.com/i2xAm1r/Iranslot-App)

## Acknowledgments

<b>This application was developed by [i2xAm1r](https://github.com/i2xAm1r/) The DNS server sets were provided by the developer and may be subject to change<b>
