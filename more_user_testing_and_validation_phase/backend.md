# The technology

To integrate with current CRMs we decided to propose a webhook.

Integration is one of the many problems of software development for government. Many different departments may have different systems and even different use cases for interacting with your application, it is often not feasible to try to integrate with every different system.

Once you accept that, there are several ways that your application can provide in order to empower external developers (AKA developers who you have no control over and no interaction with) to work with your system. The API is a great way of doing this and a well known one. However, it's not always the right solution.

The downside of the API is that the external developer has to continuously poll your system and write code that will detect changes when new data is created. While you can offset her work by writing a smarter resource that will only return the new data once, or by allowing her to send a timestamp, it's still not an optimal solution.

An oftentimes better option is to allow the developer to receive the new data in real time as it comes in. This type of integration pattern is called a web hook and is a very common and widely used pattern.

The idea is similar to a subscriber model. The developer provides your application a URL to hit when a certain event happens. Let's call this the receive URL. When that event happens, your application sends a standardized, pre-defined, documented payload to the receive URL.

At the callback to the receive URL, the developer has written code to grab data from the payload that is needed for that specific integration, and do what's needed. The rest of the data just fades away into the ether.

![](http://cl.ly/XAyK/IMG_0148.jpg)

You can check our app here: https://github.com/codeforamerica/primerpeso

