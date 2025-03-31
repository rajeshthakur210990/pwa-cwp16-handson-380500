## pwa-kit-create-app@v3.8.0 templateVersion 5.0.0 handson
npx @salesforce/pwa-kit-create-app@v3.8.0 --templateVersion 5.0.0 --outputDir projectDir
## SFCC demo pwa sandbox
https://zzab-001.dx.commercecloud.salesforce.com/ 
6d17e164-4331-482a-908e-ff8d007f7782 
RefArch 
f_ecom_zzab_001 
kv7kzm78
## SFCC demo pwa old sandbox
https://zzpe-007.dx.commercecloud.salesforce.com/
8e90cc31-f040-4dcf-95b6-2c5451c15b48
RefArch
f_ecom_zzpe_007
kv7kzm78
## cwp sbx 16
https://bfvb-016.dx.commercecloud.salesforce.com/ 
f037520f-91bd-468b-a62c-49c373836928 
Centerwell/RefArch 
f_ecom_bfvb_016 
bej569cx
## MRT config
MRT API Key: iL47gTp67k6T3i3QVrZa4FzEZTA32YI3bl8BFCOVT2A 
npx @salesforce/pwa-kit-dev@latest save-credentials --user rthakur12@humana.com --key iL47gTp67k6T3i3QVrZa4FzEZTA32YI3bl8BFCOVT2A (save MRT push creds) 
npm run push -- -m "MRT bundle 2025.03.25_1" (push to MRT, can be deployed on any env then) iL47gTp67k6T3i3QVrZa4FzEZTA32YI3bl8BFCOVT2A
## Old MRT config
npx @salesforce/pwa-kit-dev@latest save-credentials --user rajeshthakur.0123@gmail.com --key 5IBHRWZgERGgL4qSweocOsveo42FuzzVuo48vQH2qT4
npm run push -- -m "Message to help you recognize this bundle"
npx @salesforce/pwa-kit-dev@latest tail-logs --project pwakit-mrt-training-6 --environment rthakur-env
## MRT commands:
List environments: curl "https://cloud.mobify.com/api/projects/$PROJECT_ID/target/" \ --header "Authorization: Bearer $API_KEY"
List environments: curl "https://cloud.mobify.com/api/projects/pwakit-mrt-training-6/target/" --header "Authorization: Bearer 5IBHRWZgERGgL4qSweocOsveo42FuzzVuo48vQH2qT4"
## MRT Deploy bundle statuses:
Checking shared regional resources
Checking rendering service
Updating rendering service
Checking CDN
Updating CDN
Finishing deployment
## Hooks:
useCommerceApi
useEinstein
useIntl
useMultiSite
useProductSearch
useServerContext
useQueries
useEffect
useShopperBasketsMutation('createBasket')
useCurrentBasket
useCurrentCustomer
useStyleConfig
useAuthModal
useHistory
useLocation
useActiveData
useAccessToken
useLazyLoadCategories
useCategoryBulk

## Environments:
Environments without activity will be deleted
Environments not marked as Production will be automatically deleted after 30 days of inactivity.

Development
Production

## Deployments
URL Redirects
Environment variables
Logs(npx @salesforce/pwa-kit-dev@latest tail-logs --project pwakit-mrt-sample2 --environment development)
## Env settings:
Name: Development
Environment ID: development
Production Environment: Disabled
B2C Commerce Instance: zzab_001
Site IDs: RefArch
Access Control
Advanced
External Hostname: pwakit-mrt-sample2-development.mobify-storefront.com
External Domain: mobify-storefront.com
Region: US East (N. Virginia)
Cookies: Disabled
Source Maps: Enabled
Allowed IP Addresses
Proxy Configs(Proxies allow you to route HTTP requests (to APIs, for example) through a single domain in a simple, fast, and observable way. Proxy settings on the Managed Runtime are separate from proxy settings in the bundle.): Proxy: https://pwakit-mrt-sample2-development.mobify-storefront.com/mobify/proxy/api/*
Destination: https://kv7kzm78.api.commercecloud.salesforce.com/*
Proxy: https://pwakit-mrt-sample2-development.mobify-storefront.com/mobify/proxy/ocapi/*
Destination: https://zzab-001.dx.commercecloud.salesforce.com/*

Automatically follow redirects is switched oﬀ for this course. This enables the
authorization code returned from the server in the Location header to be saved. If
you leave the redirects on, requests are redirected before the tests execute to save
the authorization code, so the authorization code isn’t saved. You’ll learn more about
this later in the course.

:loudspeaker: Hey there, Salesforce Commerce Cloud community!

We’re excited to hear your thoughts on your developer experience with PWA Kit and the Composable Storefront generally! Your feedback is incredibly valuable in helping us guide our roadmap and improve our offering.

:clipboard: Take our quick survey here: [Survey](https://forms.gle/bUZNxQ3QKUcrjhV18) 

Feel free to share this survey link with your colleagues, partners, or anyone who has experience with PWA Kit. Your input will help us shape the future of our development tools.

Thank you for being a part of our community and for your continuous support! :raised_hands:

# The Retail React App

A project template that includes an isomorphic JavaScript storefront and [Progressive Web App](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps) built using [React](https://reactjs.org/) and [Express](https://expressjs.com/). It uses a modern headless architecture that enables developers to decouple front-end code from back-end systems. It leverages popular open-source libraries in the React ecosystem, such as [Chakra UI](https://chakra-ui.com/) components, [Emotion](https://emotion.sh/docs/introduction) (CSS-in-JS), [Webpack](https://webpack.js.org/), and many more.

Developers don’t have to worry about the underlying infrastructure, whether they’re developing their app locally, deploying it to a [Managed Runtime](https://developer.salesforce.com/docs/commerce/pwa-kit-managed-runtime/guide/mrt-overview.html) environment, or testing the app live.

## Requirements

-   Node 16.11 or later
-   npm 8 or later

## Get Started

To start your web server for local development, run the following command in your project directory:

```bash
npm start
```

Now that the development server is running, you can open a browser and preview your commerce app:

-   Go to http://localhost:3000/

## Localization

See the [Localization README.md](./translations/README.md) for important setup instructions for localization.

## Configuration Files

The Retail React App's configuration files are located in the `app/config` folder. For more details, see [Configuration Files](https://developer.salesforce.com/docs/commerce/pwa-kit-managed-runtime/guide/configuration-options.html) in the documentation.

## Documentation

The full documentation for PWA Kit and Managed Runtime is hosted on the [Salesforce Developers](https://developer.salesforce.com/docs/commerce/pwa-kit-managed-runtime/overview) portal.

### Useful Links:

-   [Get Started](https://developer.salesforce.com/docs/commerce/pwa-kit-managed-runtime/guide/getting-started.html)
-   [Skills for Success](https://developer.salesforce.com/docs/commerce/pwa-kit-managed-runtime/guide/skills-for-success.html)
-   [Set Up API Access](https://developer.salesforce.com/docs/commerce/pwa-kit-managed-runtime/guide/setting-up-api-access.html)
-   [Configuration Options](https://developer.salesforce.com/docs/commerce/pwa-kit-managed-runtime/guide/configuration-options.html)
-   [Proxy Requests](https://developer.salesforce.com/docs/commerce/pwa-kit-managed-runtime/guide/proxying-requests.html)
-   [Push and Deploy Bundles](https://developer.salesforce.com/docs/commerce/pwa-kit-managed-runtime/guide/pushing-and-deploying-bundles.html)
-   [The Retail React App](https://developer.salesforce.com/docs/commerce/pwa-kit-managed-runtime/guide/retail-react-app.html)
-   [Rendering](https://developer.salesforce.com/docs/commerce/pwa-kit-managed-runtime/guide/rendering.html)
-   [Routing](https://developer.salesforce.com/docs/commerce/pwa-kit-managed-runtime/guide/routing.html)
-   [Phased Headless Rollouts](https://developer.salesforce.com/docs/commerce/pwa-kit-managed-runtime/guide/phased-headless-rollouts.html)
-   [Launch Your Storefront](https://developer.salesforce.com/docs/commerce/pwa-kit-managed-runtime/guide/launching-your-storefront.html)
