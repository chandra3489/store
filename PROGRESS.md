1. Creating springBoot application "store" and adding maven dependencies
2. Creating Controller class to return index.html from resources with "Hello World" text
3. Creating a property in application.properties and reading it in the controller class
4. Getting the app running on localhost:8080
5. Creating OrderService with placeOrder method with tight coupling to Stripe Payment Service
6. To introduce dependency injection, creating payment service interface and implement it in StripePaymentService and PaypalPaymentService
7. Then, creating a constructor in order service with payment service type parameter and assigning it as local object.
8. Then, injecting dependency to the StoreApplication by passing either of the service types to orderService object, thus freeing up OrderService class to need modifications for a new payment service.