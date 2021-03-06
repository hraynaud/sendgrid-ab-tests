# A/B Test SendGrid Email
This repository demonstrate how to use [SendGrid](http://sendgrid.com)'s [categories](http://sendgrid.com/docs/API_Reference/SMTP_API/categories.html) and [statistics endpoint](http://sendgrid.com/docs/API_Reference/Web_API/Statistics/index.html) to run A/B tests. You can use this [app on Heroku](https://sendgrid-ab.herokuapp.com/), to analyze your own tests, the only requirement being you setup categories for each variable you wish to test.

The business code of this app is really found in [index.html](https://github.com/nquinlan/sendgrid-ab-tests/blob/master/public/index.html), which does all the computation and makes all the requests. The server in this app, is only used to guarantee HTTPS and proxy [SendGrid's Stats Endpoint](http://sendgrid.com/docs/API_Reference/Web_API/Statistics/index.html), so it can be accessed by Javascript.

**Further explanation of this app and its methods can be found in [A/B Testing Explained and Used in Transactional Email](http://sendgrid.com/blog/ab-testing-explained-used-transactional-email/) on the SendGrid Blog.**

![YAY STATISTICS](https://sendgrid.com/blog/wp-content/uploads/2014/02/YAY-STATISTICS.gif)
