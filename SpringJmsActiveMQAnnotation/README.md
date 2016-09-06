Spring4MVCJmsActiveMQExample
------------------------------
@Ref: http://websystique.com/springmvc/spring-4-mvc-jms-activemq-annotation-based-example/


Spring provides first-class support for JMS, enabling applications integration using standard based messaging. In this post, we will build Spring 4 MVC application communicating with another Spring-based application, using JMS through Apache ActiveMQ. For a general introduction on JMS itself, please refer to post Spring 4 + JMS+ActiveMQ Annoataion based Example. We will try to touch them in this post as well.

You can quickly check the WebConsole [available at http://localhost:8161/admin/ with credentials admin/admin.


Now go to ActiveMQ webconsole and check the queues on http://localhost:8161/admin/queues.jsp. You will see both the queue’s and an enqueued message on order-queue. Also notice that web-shop application is rgistered as a consumer on order-response-queue [as it is listing on this queue].


On our application side, you can check the order status. It is in created state [because it is not yet processed by Inventory application , we did not deploy it yet].

