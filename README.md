# Google Analytics Setup Account

### Setup Account
- goto your [google analytics](https://analytics.google.com/analytics/web/) accout
- on admin setting create an account and fill up the form
- save and get tracking **ID** and **Code**
- Goto your website ex: `example.com` place the code before the end of html header tag.
**ex:**

        <html>
            <head>
               // place google analytics code here
            </head>
- to see if the page is updated go to to site homepage and **right click** on the browser and select `view page source`
- add google chrome extension
- to see real time reports your real time reports go back to your google analytics account. `Goto > reports > overview` 
wait for a minute process the data

### Setup Goals
- go to admin section on `view section` click `goals`
- create a new goals and select your configuration for now we use `custom` and continue.
**ex** form
> **Goal Description**
> Name : `Purchase Ex.`
> Goal Slot ID : `your selected id`
> Select your type: `i select here is Destination`
> **Goal Details**
> Destination : `Begins with` : `/checkout/order-received/` this will be your url checkout page for ex. `click save`
> to track your goals `reports` and click `convertions`

[![Alt text](https://img.youtube.com/vi/ZM-ZH3m7zSA/mqdefault.jpg)] (https://www.youtube.com/watch?v=ZM-ZH3m7zSA)

**visit video tuitorial [here](https://www.youtube.com/watch?v=ZM-ZH3m7zSA)**

# GTM - GTM Account Setup
For websites with more complex tracking needs (events, etc)

### step 1
- goto to your [tag manage](https://tagmanager.google.com/) account
- on the top right of the page click `create accout`
- on **Setup Account** enter the account name Ex: `Total Service` then click `CONTINUE`.
- on **Setup Container** enter container name Ex: `Total Service` click `WEB` then click `CREATE`
- accept the terms and click `YES`
- this will return a code that will insert to your website
     
      <html>
        <head>
            // code for the head tag. place as high in header tag
        </head>
        <body>
            // code for body tag. place immediately after opening <body> tag

### step 2

- on **VARIABLE MENU SECTION** `create` a new variable called `GA - Tracking ID`
- on Variable Configuration choose a `variable type` and select `Google Analytics Settings`
- copy your `Tracking ID` on your Google Analytics Account and place on request field `Tracking ID` leave the cookie domain and click `SAVE`
- on your **TAG MENU SECTION** `create` a tag called `GA - Pageview` 
- on Tag Configuration choose a `tag type` and select `Google Analytics`
- on `Track Type` select `Page View` and for Google Analytics Settings select `{{GA - Tracking ID}}`
- Triggering should be `All Pages` and then click `SAVE`
- on the up right of the page click `SUBMIT`
> Version Name Ex: `Initial Version`
> Version Description Ex: `Initial Version`
- click `PUBLISH`

### step 3

- go back to [Google Analytics](https://analytics.google.com/analytics/web/) account
- click `View Setting`
- rename **View Name** as `Main View`
- set the `filtering`
- click `Bot Filtering` if site is not site search and click `SAVE`
- create another view and rename `Unfiltered View` set Time Zone and click `CREATE`
- on ADMIN upper right page select `Main View`
- click `filters`, add filter Filter Name Ex: `Include Hostname`
- select `Custom` filter type
- select `include`, Filter Field Ex: `Hostname`, Filter Pattern Ex: `example.com` and click `SAVE`
- to make sure if all set on ADMIN property column SELECT `Tracking Info` > `Referral Exclusion List`

visit the video tuitorial [here](https://www.youtube.com/watch?v=hgIcXHnmS3w)