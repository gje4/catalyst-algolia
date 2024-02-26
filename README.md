## ****How to Integrate Algolia SearchBox into Catalyst


## **Introduction**
The introduction consists of 2-3 sentences to orient the reader. State the guide’s purpose.

Developers can quickly integrate Algolia search into the BigCommerce frontend Catalyst to enable search across all products.
This guide walks through the basic integration and provides files that can be copy and pasted into Catalyst CORE app.




## **Prerequisites**
To complete the guide, you will need the following:
A BigCommerce Store
Catalyst setup, https://github.com/bigcommerce/catalyst
An Algolia account

Experience using Next.js

This guide assumes the merchant has the following configured:

A functioning BigCommerce store.
Store settings, including Catalog, The algolia app installed, https://www.bigcommerce.com/apps/algolia-search-discovery/

## Requirements

- Node.js 18+
- `npm` (or `pnpm`/`yarn`)

## **Steps**

1. Once you have catalyst running.  Grab the quick search files from here.
2. Add algolia keys to .env.
`  ALGOLIA_APP_ID=
   ALGOLIA_APP_KEY=`
3. Import `npm i react-instantsearch` , `npm i -S algoliasearch`
4. Add the files algoliasearchbox.tsx and algoliaSearchHits.tsx to QuickSearch componenet.
   ![Screenshot 2024-02-21 at 3.00.19 PM.png](..%2F..%2F..%2F..%2F..%2F..%2Fvar%2Ffolders%2Ffq%2Fgk1dfgmn1qdd1dcgb9sfphn40000gq%2FT%2FTemporaryItems%2FNSIRD_screencaptureui_aYRqvu%2FScreenshot%202024-02-21%20at%203.00.19%20PM.png)
5. Update the code in index.tsx to use the code from here _>>>.
6. Update the algoliaClient in index.tsx to use your store keys and the correct indexName.  
By default the algolia app names the index BigCommerce.  You can then delete the _actions directory.
![Screenshot 2024-02-25 at 9.01.16 PM.png](..%2F..%2F..%2F..%2Fvar%2Ffolders%2Ffq%2Fgk1dfgmn1qdd1dcgb9sfphn40000gq%2FT%2FTemporaryItems%2FNSIRD_screencaptureui_1QGUYP%2FScreenshot%202024-02-25%20at%209.01.16%20PM.png)
7. Run the app pnpm run dev, and check the quick search box to see data returned from algolia.



## Resources

