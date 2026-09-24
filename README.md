# AI Auto Trader

Fresh Android + Python backend foundation for autonomous trading against **Binance Testnet only**.

## Safety
This initial build cannot place real-money orders. The backend explicitly uses Binance Testnet and the Android UI labels the environment.

## Backend
```bash
cd backend
python -m venv .venv
pip install -r requirements.txt
uvicorn main:app --reload
pytest
```

Set `BINANCE_TESTNET_API_KEY` and `BINANCE_TESTNET_API_SECRET` only for Testnet credentials.

## Android
Requires Android Studio/SDK and Gradle. The project uses compileSdk 35, minSdk 26, Kotlin 2.1.20, Android Gradle Plugin 8.8.2.
