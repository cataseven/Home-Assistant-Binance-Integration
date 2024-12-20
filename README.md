# Binance Wallet Balances and Price Tracking Integration for Home Assistant

This integration allows you to add cryptocurrency prices and your wallet balances from your Binance account to Home Assistant.

## Installation

Download from HACS or 

Copy paste files to your HA folder: custom_components/binance/ or

Add custom repo from HACS via https://github.com/cataseven/Home-Assitant-Binance-Integration.git

Clean your browser cache, restart HA and...

1. Create an API key and API secret for your Binance account. <strong><span style="color: red;">IMPORTANT</span></strong> Please only use Read Only API. If you do not want to create sensor for your Wallet Balance do not check "Permits Universal Transfer" option. Use IP restriction for max safety! DO NOT SHARE YOUR API KEY and SECRET KEY with ANYONE!! It is your own responsibility to manage your api credentials!
![2024-11-21 15_28_27-Greenshot image editor](https://github.com/user-attachments/assets/d1fb4449-024e-4342-b4e6-c8827f530182)
2. In Home Assistant, go to **Settings** > **Integrations** > **Add Integration**.
3. Search for and select **Binance**.
4. Enter your API key and API secret.
5. Select the coin pairs you want to track.
6. Click **Submit**.

## Sensors

This integration creates the following sensors:

* **Binance Wallet Balance:** A sensor that shows the balances in your Binance wallets. Please see attributes of sensor. You can see your total balances as state and market based wallets as attributes.
![2024-11-22 10_27_06-Greenshot image editor](https://github.com/user-attachments/assets/36535afc-f4ca-4eaf-b59c-ac294ee3d625)

* **Binance Futures {symbol} Price:** A price sensor for each selected futures pair. Please see attributes of sensor: "Price" and "Price Change % 24h"
* **Binance Spot {symbol} Price:** A price sensor for each selected spot pair. Please see attributes of sensor: "Price" and "Price Change % 24h"
  ![2024-11-22 10_32_14-Developer Tools – Home Assistant](https://github.com/user-attachments/assets/cde7d0b5-6cc5-40d6-8125-a1b573694b51)



## Supported Coin Pairs

This integration supports all coin pairs that are supported by Binance Spot and COIN Futures Markets.
![2024-11-22 10_33_37-Settings – Home Assistant](https://github.com/user-attachments/assets/00c6fe96-9293-4b88-bdd0-ec967f81c60b)

![2024-11-22 10_33_50-Settings – Home Assistant](https://github.com/user-attachments/assets/7f8d535c-d458-4424-a0da-34df34fc0868)


## Troubleshooting

If you encounter any issues, please feel free to ask for help.

## Contributing

If you want to contribute to this integration, please visit the GitHub repository.

## License

This integration is licensed under the GNU GENERAL PUBLIC LICENSE v3
