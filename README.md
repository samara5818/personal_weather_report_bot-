# 🌦️ Personal Weather Report Bot

This project provides weather recommendations using **web scraping** and **Selenium automation** to send reminders via **WhatsApp** and **email**. The script checks the weather conditions in a city and notifies the user whether an umbrella is needed.

## 🚀 Features

- Scrapes real-time weather data from **Google Weather**.
- Sends personalized **WhatsApp messages** using Selenium.
- Sends **email reminders** via SMTP.
- Schedules daily reminders at a specific time.

## 🛠️ Prerequisites

Ensure you have the following installed:

- **Python 3.8+**

- **Required Python libraries**:
  - `schedule`
  - `smtplib` (built-in)
  - `requests`
  - `beautifulsoup4`
  - `selenium`

- **Edge WebDriver**:
  - Download from [Edge WebDriver Page](https://developer.microsoft.com/en-us/microsoft-edge/tools/webdriver/).
  - Ensure `msedgedriver.exe` matches your Edge browser version.

## 📦 Installation

### 1. Clone the repository:
```bash
git clone https://github.com/your-repo/weather-reminder-bot.git
cd weather-reminder-bot
```
### 2. Install required libraries:
```bash
pip install schedule requests beautifulsoup4 selenium
```
### 3. Place the Edge WebDriver:
- Place the Edge WebDriver (msedgedriver.exe) in the project directory or specify its path in the script.

## 🔧 Configuration

Update the following in the script when prompted:

- **City Name**: Enter the city for which you want weather updates.

- **Email Credentials**:
  - **Email**: Your Gmail address.
  - **Password**: Generate and use an **App Password** (for security).

- **WhatsApp Phone Number**: Provide the number in **international format** (e.g., `+1234567890`).

- **Scheduled Time**: Specify the **hour** and **minute** for daily email reminders.

## 📝 How to Run

### Run the script:
```bash
python weather_reminder.py
```
### Follow the prompts to:
- Enter your **city name**.
- Provide **email credentials**.
- Set the **notification time** and **phone number**.
- Scan the **WhatsApp Web QR code** when prompted.

### The program will:
- Check **weather conditions**.
- Send **WhatsApp** and **email reminders** based on the forecast.
- Schedule a **daily email reminder**.

## 🖥️ Sample Output

### Console Output:
```plaintext
🌍 Hey there! What's the name of your city? 🏙️: Los Angeles
📧 Drop your email address here to stay updated: example@gmail.com
🔒 Enter your email password (safe with us 🤞): ****
Enter hours in 24 hours format: 8
Enter mins in 24 hours format: 30
Enter the phone number with country code: +1234567890
✅ Message sent successfully!
✅ Email Sent Successfully!
Scheduled umbrella reminder.
Today's weather in Los Angeles is Mostly sunny. No umbrella needed.
```

### Whatsapp message:
```plaintext
☀️ Good news! No rain today. 😎

Weather for today in Los Angeles: Mostly sunny
🌡️ Temperature: 25°C

Enjoy your day! 🌈
Your Weather Bot 🤖
  
```

### Email Message:
Subject: Umbrella Reminder

Body:
```plaimtext
☀️ Good news! No rain today. 😎

Weather for today in Los Angeles: Mostly sunny
🌡️ Temperature: 25°C

Enjoy your day! 🌈
Your Weather Bot 🤖
```

## 🛡️ Security Notes

- Use **App Passwords** instead of plain email passwords for Gmail.  
  Enable **2-Step Verification** and generate an App Password [here](https://myaccount.google.com/apppasswords).

- Ensure **WhatsApp Web** remains logged in during the script execution.

## ⚠️ Troubleshooting

### "Unable to locate WebDriver" Error:
- Verify that `msedgedriver.exe` is in the correct path and matches your Edge browser version.

### "No such element" Error:
- Ensure **WhatsApp Web** has fully loaded before proceeding.
- Increase the wait time in `WebDriverWait`.

### SMTP Authentication Error:
- Enable **"Allow less secure apps"** or use **App Passwords** for Gmail.

---

## 🎉 Future Improvements
- Add support for other browsers (e.g., Chrome).
- Use APIs (like **OpenWeatherMap**) for faster and more reliable weather data.
- Integrate **push notifications** for mobile devices.

---

## 💡 Dependencies
- `schedule`: For task scheduling.
- `smtplib`: For sending emails via SMTP.
- `requests`: For web scraping.
- `beautifulsoup4`: To parse HTML content.
- `selenium`: For automating WhatsApp Web.

---

## 🤝 Contribution
Contributions are welcome! If you'd like to add new features, fork the repository, make changes, and submit a pull request.

