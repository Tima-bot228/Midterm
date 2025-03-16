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

Примеры работы 
```
Enter payment method (Halyk Bank || Forte Bank || Kaspi Bank): halykbank
Enter amount: 10000
Are you sure? Enter '1234' to confirm payment.
1234
Processing Halyk Bank payment: 10000.0₸`
```
Не правильный код 
```
Are you sure? Enter '1234' to confirm payment.
5678
Payment canceled. Incorrect confirmation code.
```
