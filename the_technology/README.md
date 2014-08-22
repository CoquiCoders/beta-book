# The technology

The application is a node.js webapp.
Here is the repo: https://github.com/CoquiCoders/bizwallet

To integrate with current CRMs we decided to propose a webhook.

Webhooks are sometimes referred to as “Reverse APIs,” as they give you what amounts to an API spec, and you must design an API for the webhook to use. The webhook will make an HTTP request to your app (typically a POST), and you will then be charged with interpreting it.

Agencies will be giving us a place to send it as events happen.
