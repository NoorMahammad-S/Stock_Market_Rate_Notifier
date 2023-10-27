# Stock_Market_Rate_Notifier
This Python script fetches the stock price of a specified company &amp; sends news alerts to your phone using Twilio if the stock price increases or decreases significantly.

## Prerequisites

Before running the script, you need to obtain API keys and set up a Twilio account. You will also need to install the required Python packages listed in the `requirements.txt` file.

### Obtaining API Keys

- **Alpha Vantage API Key:** You can obtain an API key from [Alpha Vantage](https://www.alphavantage.co/) by signing up for a free account.

- **News API Key:** You can obtain an API key from [NewsAPI](https://newsapi.org/) by signing up for a free account.

- **Twilio Account SID and Auth Token:** You need to sign up for a Twilio account, obtain your Account SID and Auth Token, and set up a virtual Twilio phone number.

## Installation

1. Clone this repository to your local machine.

2. Install the required Python packages using pip:

   ```bash
   pip install -r requirements.txt
   ```

3. Create a `secrets.py` file in the same directory and add your API keys and Twilio account information as follows:

   ```python
   STOCK_API_KEY = "YOUR_ALPHA_VANTAGE_API_KEY"
   NEWS_API_KEY = "YOUR_NEWSAPI_API_KEY"
   TWILIO_SID = "YOUR_TWILIO_ACCOUNT_SID"
   TWILIO_AUTH_TOKEN = "YOUR_TWILIO_AUTH_TOKEN"
   VIRTUAL_TWILIO_NUMBER = "YOUR_VIRTUAL_TWILIO_NUMBER"
   VERIFIED_NUMBER = "YOUR_PHONE_NUMBER"
   ```

   Make sure to add `secrets.py` to your `.gitignore` file to keep it private.

## Usage

Run the script:

```bash
python stock_price_notifier.py
```

The script will check the stock price for the specified company (e.g., TSLA for Tesla Inc). If the stock price change is greater than 1%, it will fetch news articles related to the company and send them to your phone number using Twilio.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to Alpha Vantage and NewsAPI for providing free access to financial and news data.
- Thanks to Twilio for their communication services.

Feel free to customize and improve this script as needed. If you have any questions or issues, please open an [issue](https://github.com/NoorMahammad-S/your-repo-name/issues) on GitHub.

Happy investing!
