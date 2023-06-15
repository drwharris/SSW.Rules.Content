---
type: rule
title: Do you know to use Configuration over Key Vault
uri: know-configuration-versus-key-vault
authors:
  - title: Andrew Harris
    url: https://ssw.com.au/people/andrew-harris
  - title: Matt Wicks
    url: https://ssw.com.au/people/matt-wicks
  - url: https://ssw.com.au/people/william-liebenberg
    title: William Liebenberg
related:
  - store-your-secrets-securely
created: 2023-06-15T05:22:41.457Z
guid: fe25e667-cfe2-40b7-b0c9-c66a181a8a50
---
We all know that we should [Store Secrets Securely](https://www.ssw.com.au/rules/store-your-secrets-securely/) using Key Vault, but did you know that you can abstract Key Vault out of your application code and leave developers to only have to deal with Configuration?
        

<!--endintro-->

A feature of Azure AppService is the ability to [use secrets from Key Vault as Configuration values](https://learn.microsoft.com/en-us/azure/app-service/app-service-key-vault-references). This allows you to setup a link between your AppService and a Key Vault and have Configuration values point to a Key Vault Entry.

So now rather than developers having to think about if a value is a secret or configurations, its always configuration. It just might have its value stored securely in Key Vault.