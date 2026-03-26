# 📈 Stock Price Service (Backend)

A Spring Boot based REST API that fetches stock prices and provides a fallback mechanism for reliability.

---

## 🚀 Features

* 🌐 REST API for fetching stock prices
* ⚡ WebClient integration (non-blocking API calls)
* 🔄 Fallback mechanism (when external API fails)
* 🧾 Logging with SLF4J
* ❗ Global exception handling

---

## 🏗️ Project Structure

```bash
src/main/java/com/mohsin/stockpriceservice/
 ├── controller/
 ├── service/
 ├── exception/
 ├── config/
 └── StockPriceServiceApplication.java
```

---

## ⚙️ Tech Stack

* Java 17+
* Spring Boot
* Spring Web
* Spring WebFlux (WebClient)
* Lombok
* Maven

---

## ▶️ Run the Application

```bash
mvn spring-boot:run
```

---

## 🌐 API Endpoint

```bash
GET http://localhost:8080/api/stocks/price?stockName=TESLA
```

---

## ✅ Example Response

```json
245.75
```

---

## ❗ Error Response

```json
"Stock service unavailable. Try later."
```

---

## 🔐 Notes

* External API (`sbe.biz`) is not reliable
* Fallback logic is implemented for demo purposes
* You can integrate real APIs like AlphaVantage

---

## 📊 Logging

* INFO → Request tracking
* ERROR → API failure logs

---

## 🚀 Future Improvements

* 🔄 Circuit Breaker (Resilience4j)
* 📦 Caching (Redis)
* 🔐 Security (JWT)
* 📡 Real stock API integration

---

## 👨‍💻 Author

**Md Mohsin Haider**
