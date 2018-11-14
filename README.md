# Google Analytics Setup Account

### Setup Account
- goto > [google analytics](https://analytics.google.com/analytics/web/)
- create an account and fill up the form
**ex:** form
> Account Name: `Company Name Ltd.`
Website Name : `exmaple.com`
Website Url : `http / https`
Reporting Time Zone : `select right timezone`
save and get tracking **ID** and **Code**


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