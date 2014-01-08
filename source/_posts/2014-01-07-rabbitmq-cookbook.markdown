---
layout: post
title: "RabbitMQ Cookbook"
date: 2014-01-07 20:20
comments: true
categories: learning 
tags: 
- learning
- technology
---
{% img left /images/rabbitmq_cookbook.jpg 200 %}
I recently finished my first go at being a technical reviewer for a technology book: the [RabbitMQ Cookbook][cookbook]. I kind of 'happened' into reviewing from some of the tech talks, blog posts and [slide decks][slides] I have done on the subject of [RabbitMQ][rabbitmq]. An editorial representative from [Packt Publishing][packt] contacted me to see if I would be interested in being a technical reviewer for the up comming book -- and the adventure began.

A technical reviewer looks primarily at the technical correctness and ease of understanding in each of the chapters. There are plenty of opportunities to offer suggestions for improvements to the author(s).

## Technical Reviewing

TBD

## The Book

This book is an excellent resource for anyone looking to use RabbitMQ (or any other AMQP server for that matter...) for queuing/integration. Most modern software components [pass messages][messages] to other components, not data. I thoroughly enjoyed reviewing this book and learn some new RabbitMQ tricks in the process. The format uses a clean cookbook of recipe description, how to implement the recipe, and how the recipe works. It makes finding a solution to a queuing challenge a quick and easy process.

This book comprises over 265 pages and 70 recipes for a myriad of integration solutions. [Sigismondo][sigis] and [Gabriele][gab] did a great job of showing code examples for Java, C#, Python as well as others languages. In addition to the examples, they also show how to properly manage a RabbitMQ server and deploy it to the cloud.

Here is a brief table of contents:

	1. Working with AMQP
	2. Going beyond the AMQP Standard
	3. Managing RabbitMQ
	4. Mixing Different Technologies
	5. Using RabbitMQ in Web Applications
	6. Developing Scalable Applications
	7. Developing High-Availability Applications
	8. Performance Tuning for RabbitMQ
	9. Extending RabbitMQ Functionality
	10. RabbitMQ on AWS
	11. AMQP and Cloud Computing - RabbitMQ on PAAS
	12. Managing RabbitMQ Error Conditions

One of my favorite recipes in the book is for auto scaling RabbitMQ servers on AWS -- it is a formula you can use for not only RabbitMQ but other EC2 instances on AWS.

## Conclusion

If you want a flexible/scalable backbone for your Enterprise application (or future Enterprise application) -- RabbitMQ is a great option, and this book is a great head start for that option.

Technical reviewing is also a great way to get involved with a technology that you like!

[cookbook]: http://bit.ly/1b2OwRo
[rabbitmq]: http://www.rabbitmq.com/
[packt]: http://www.packtpub.com/
[slides]: https://speakerdeck.com/switchspan/rabbitmq-and-easynetq
[sigis]: http://www.packtpub.com/authors/profiles/sigismondo-boschi
[gab]: http://blog.indigenidigitali.com/tag/gabriele-santomaggio/
[messages]: http://en.wikipedia.org/wiki/Message_passing
