---
layout: post
title:  "How to setup a Hydrogen Store localy with a development store."
date:   2024-03-21 16:00:00 +0200
categories: jekyll update
hero: /yurith-says/assets/images/welcome/woman-working-computer.png
# image rendered with the AI on this page: https://hotpot.ai/art-generator
---

How to setup a Hydrogen Shopify store in a local environment with the products from a development store.

If you are looking for how to setup a Hydrogen store as a developer without paying a monthly fee of your store which is necessary when installing a Hydrogen app on your store to get access to your products.  Here I will describe how I did it.

What you need:
- Have a development store
- Install the headless app on your dev store

1. On your terminal / or preferred code editor

    1. inside a directory of your choice.
    2. command: npm create @shopify/hydroge@latest
    3. follow the steps
    4. set sample data from Mockup.shop
    5. go to your .env file and add the values of:

        1. ADD PRIVATE_STOREFRONT_API_TOKEN and PUBLIC_STOREFRONT_API_TOKEN to your .env file. PUBLIC_STORE_DOMAIN was already set by default, otherwise add it as well.
        2. set your personal info:
            PUBLIC_STORE_DOMAIN= "yourdevstore.myshopify.com"
            PRIVATE_STOREFRONT_API_TOKEN= (here your API number which you will find on your headless installed app on your dev store)
            PUBLIC_STOREFRONT_API_TOKEN= (here your API number which you will find on your headless installed app on your dev store)
    6. command: npm run dev

    Voila! you will see your Mockup.store working with the products you have on your dev store.

    Let me know if this short post was useful and about what other topics you would like to write about. Thanks for reading.