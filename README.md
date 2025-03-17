# Midterm Exam – Online Payment Gateway & Coffee Shop Simulator

## Описание
Этот проект реализует две системы с использованием шаблонов проектирования:

1. **Online Payment Gateway** (60 баллов)  
   - Позволяет выбирать метод оплаты (CreditCard, PayPal).  
   - Использует **Factory Method** для создания платёжных объектов.  
   - Запрашивает **код подтверждения** перед оплатой.  

2. **Coffee Shop Simulator** (40 баллов)  
   - Позволяет заказывать кофе и добавлять ингредиенты.
   - Использует **Factory Method** для создания базовых напитков.  
   - **Decorator** позволяет динамически добавлять молоко, карамель и другие добавки.
   - Допалнительно выводит суммы в (₸ || ₽ || $)

**Примеры работы**
```
Enter payment method (Kaspi Bank || PayPal || Crypto): k
Enter amount: 500000
Enter details (Card Number || PayPal Email || Crypto Wallet): 4433434456785236
Are you sure? Enter '1234' to confirm payment.
1234
Processing Kaspi Bank payment: 500000.0₸
Transaction 1dc455a6-aecf-4c8e-b80f-c6efc4af5566 - COMPLETED

Transaction History:
1dc455a6-aecf-4c8e-b80f-c6efc4af5566 - COMPLETED

```
**Не правильный код**
```
Enter payment method (Kaspi Bank || PayPal || Crypto): k
Enter amount: 500000
Enter details (Card Number || PayPal Email || Crypto Wallet): 1234567891234567
Are you sure? Enter '1234' to confirm payment.
1452
Payment canceled.
Transaction 4f368a6c-ee27-41b2-9034-73609b3e0ebd - CANCELED

Transaction History:
4f368a6c-ee27-41b2-9034-73609b3e0ebd - CANCELED

```

**Пример работы (Coffee Shop Simulator)**
```
Choose coffee (Espresso / Cappuccino): Espresso
Add milk? (yes/no): yes
Add caramel? (yes/no): no
Your order: Espresso with Milk
Total cost: 500.0₸
Total cost: 100.0₽
Total cost: 1.0$
```
