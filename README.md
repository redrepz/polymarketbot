# Polymarket Arbitrage Bot (BTC 5-Min Fast-Loop) 🚀

Dieser Bot ist darauf optimiert, Preisdifferenzen (Divergenzen) zwischen dem realen Bitcoin-Kurs (Binance) und den Prognosemärkten auf Polymarket in Echtzeit zu erkennen.

## 📈 Strategie
Der Bot nutzt ein Zeitfenster von ca. **5ms - 20ms**, das entsteht, weil Polymarket-Preise oft verzögert auf schnelle BTC-Sprünge reagieren.
1. **Echtzeit-Feed:** Abfrage des BTC/USDT Preises über Binance API.
2. **Orderbuch-Check:** Überwachung der Token-ID (JA/NEIN) auf Polymarket.
3. **Execution:** Automatischer Kauf, wenn die Divergenz einen Schwellenwert überschreitet.

## 🛠 Installation
1. Repository klonen oder Dateien in einen Ordner kopieren.
2. Virtuelle Umgebung erstellen:
   ```bash
   python3 -m venv venv
   source venv/bin/activate
