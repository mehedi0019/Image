[readme.md](https://github.com/user-attachments/files/23053379/readme.md)
# Facebook ID Auto Reset Code Sender

A powerful automation tool for checking Facebook account validity and sending reset codes via SMS. Perfect for bulk phone number verification and account recovery operations.

![Main Interface](https://raw.githubusercontent.com/mehedi0019/Image/main/a.png)


✨ Features


🔍 Bulk Number Verification

- Check multiple phone numbers at once for associated Facebook accounts
- Automated verification process runs in parallel
- Real-time status updates for each number

📱 Automatic Reset Code Sending

- Automatically sends SMS reset codes when available
- Only numbers with SMS recovery option enabled are marked as valid
- Numbers without SMS option are marked as invalid (even if account exists)
- Numbers without Facebook accounts are marked as "Not Found"

📊 Smart Categorization

- ✅ Valid: Account exists AND SMS recovery available, reset code sent successfully
- ❌ Invalid: Account exists BUT SMS recovery option not available/disabled
- ⚠ CAPTCHA: Manual verification required (flagged for manual processing)
- ❓ Not Found: No Facebook account associated with number

🌐 Headless Mode

- Run browsers in background for better performance
- Reduced resource usage Faster processing speeds

📁 Flexible Input Methods

- Manual Entry: Paste numbers directly (one per line)
- CSV Import: Bulk import from CSV files

📝 Comprehensive Logging

- Session-based log files
- Master log for cumulative tracking
- Detailed status information for each number

⚡ Multi-Threading Support

- Process 1-35 numbers concurrently
- Configurable thread count for optimal performance
- Real-time progress tracking with speed and ETA

💾 Auto-Save Results

- Results automatically saved after each session
- CSV format for easy data manipulation
- Timestamped session logs

🖼 Screenshots

Processing View


![Processing Image](https://raw.githubusercontent.com/mehedi0019/Image/main/b.png)

Results Summary


![Result Summery](https://raw.githubusercontent.com/mehedi0019/Image/main/c.png)

📥 Installation

**Prerequisites**

- Windows 10/11
- Google Chrome browser (latest version)
- Internet connection

**Download & Setup**

1. **Download the Application**

   Download the latest release from the Releases section

2. **Extract Files**

   Extract the ZIP file to your desired location

   No installation required - portable application

3. **First Run**

   Double-click `fb_reset.exe` to launch

   The application will auto-download required Chrome drivers

📋 Usage Guide

**Method 1: Manual Input**

- Select "✏ Manual Input" option
- Paste phone numbers in the text box (one per line)
- Click "Browse Output Folder" and select where to save results
- Configure settings (threads, headless mode)
- Click "▶ Start Processing"

**Method 2: CSV File**

1. Select "📄 Load from CSV File" option

2. Click "Browse CSV File" and select your CSV file

- Phone numbers should be in the first column
- No header required

**Example format:**

```
8801234567890
8801987654321
8801555666777
```

3. Select output folder

4. Configure settings

5. Click "▶ Start Processing"

📊 Understanding Results

**Output Files**

Results are saved in two formats:

- Master Log (`fb_reset_master_log.csv`)
  - Cumulative log of all sessions
  - Contains timestamp for each session
  - Sessions separated by "---" rows
  - Useful for long-term tracking

- Session File (`fb_reset_session_YYYYMMDD_HHMMSS.csv`)
  - Individual session results
  - Timestamped filename
  - Easy to import into spreadsheets or other tools

**Result Categories Explained**

| Category | Icon | Description | Example Scenario |
|---|---:|---|---|
| Valid | ✅ | Facebook account exists AND SMS recovery is enabled. Reset code sent successfully. | User has account with phone number linked and SMS recovery enabled |
| Invalid | ❌ | Facebook account exists BUT SMS recovery option is not available or disabled. | User has account but disabled SMS recovery or only has email recovery |
| CAPTCHA | ⚠ | CAPTCHA verification appeared during processing. Manual intervention required. | Facebook detected automation and requires human verification |
| Not Found | ❓ | No Facebook account is associated with this phone number. | Phone number has never been linked to any Facebook account |

**Important Notes**

- Valid doesn't just mean "account exists" - it means SMS reset code was successfully sent
- Invalid can include accounts that exist but don't have SMS recovery enabled
- Not Found specifically means no account is linked to that number at all

⚙ Configuration

**Concurrent Threads**

- Range: 1-35 threads
- Default: 3 threads
- Recommended:
  - 3-5 threads for standard PCs
  - 8-10 threads for high-end systems
- Monitor CPU/RAM usage when increasing

**Headless Mode**

- Enabled: Browsers run in background (faster, less visible)
- Disabled: See browser windows (useful for debugging)
- Recommendation: Enable for production use

🚀 Performance Tips

1. **Optimal Thread Count**

- Start with 3-5 threads
- Increase gradually based on system performance
- Monitor CPU and RAM usage
- Higher thread count = faster but more resource-intensive

2. **Network Considerations**

- Stable internet connection required
- VPN may slow down processing
- Some IP addresses may trigger CAPTCHA more frequently
- Consider using residential proxies for better success rates

3. **Best Practices**

- Use headless mode for better performance
- Process in batches of 100-500 for large lists
- Close other browser instances before running
- Allow antivirus exceptions if needed
- Run as administrator for best compatibility

🔧 Troubleshooting

**Common Issues**

- "Chrome driver error"
  - Ensure Google Chrome is installed and up-to-date
  - Tool auto-downloads the correct driver
  - Try running as administrator

- High CAPTCHA Rate
  - Lower concurrent threads (try 2-3)
  - Use VPN or proxy
  - Process in smaller batches
  - Add delays between sessions

- Application Won't Start
  - Run as administrator
  - Check antivirus/firewall settings
  - Ensure all files are extracted
  - Install Visual C++ Redistributable if prompted

- Numbers Not Processing
  - Verify phone number format (include country code)
  - Check internet connection
  - Ensure output folder has write permissions
  - Review status log for specific errors

- Slow Processing Speed
  - Enable headless mode
  - Close unnecessary applications
  - Check internet speed
  - Reduce concurrent threads if system is overloaded

- High "Invalid" Count
  - This is normal - many accounts don't have SMS recovery enabled
  - Invalid = account exists but SMS option unavailable
  - Only "Not Found" means no account at all

🛠 Technical Details

**Built With**

- Python 3.x - Core language
- Tkinter - GUI framework
- Selenium - Browser automation
- Pandas - Data processing
- ChromeDriver - Browser control

**System Requirements**

- OS: Windows 10/11 (64-bit)
- RAM: 4GB minimum, 8GB recommended
- Storage: 200MB free space
- Browser: Google Chrome (latest version)
- Internet: Stable broadband connection

🔐 License & Activation

This software is protected by a device-based licensing system. Each installation requires activation.

**Getting a License**

- Run the application for the first time
- Copy your Device ID from the activation popup
- Contact developer via Telegram: @mehedi00199
- Provide your Device ID for activation
- Restart application after receiving activation confirmation

**License Terms**

- ✅ Single device license
- ✅ Lifetime updates
- ✅ Technical support
- ❌ No refunds after activation
- ❌ Non-transferable

📞 Support & Contact

**Developer**

- Mehedi Hasan

**Get Help**

- 💬 Telegram: @mehedi00199
- 🔧 Tool Support: Clone ID Tool
- 💼 Buy/Sell IDs: Clone ID Buy/Sell

**Reporting Issues**

When reporting issues, please include:

- Operating system version
- Chrome version
- Error message or screenshot
- Steps to reproduce the problem
- Log file (if available)

⚠ Disclaimer

This tool is intended for educational and legitimate account recovery purposes only.

**User Responsibilities**

- ✅ Comply with Facebook's Terms of Service
- ✅ Obtain proper authorization before processing phone numbers
- ✅ Follow local laws and regulations regarding data processing
- ✅ Use the tool ethically and responsibly
- ✅ Respect privacy and data protection laws

**Legal Notice**

The developer is not responsible for misuse or consequences arising from improper use

Users assume full responsibility for their actions

This tool should not be used for unauthorized access or malicious purposes

Bulk processing may violate platform terms - use at your own risk

🙏 Acknowledgments

Special thanks to:

- Selenium WebDriver development team
- Python community and contributors
- All beta testers and users
- Open-source libraries used in this project

🔄 Version History

**Latest Release**

Check the Releases page for the latest version

Download includes all necessary files

No additional dependencies required

🌟 Contributing

While this is a closed-source project, feedback and suggestions are welcome:

- Report bugs via Telegram
- Suggest features in the tool support group
- Share your use cases and experiences

📧 Business Inquiries

For licensing, bulk orders, custom development, or business partnerships:

Contact via Telegram: @mehedi00199

<div align="center">

Made with ❤ by Mehedi Hasan

⭐ Star this repo if you find it useful!

Telegram • Tool Support • Trading Group

</div>

