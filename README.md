# cv
First of all we need to create a resource group:
![res_gr1](https://github.com/perseptron/cv/assets/30828895/9023bdb5-b47d-45a3-93b7-7684bb888940)

Select your subscription, give to your resource group a meaningful name, choose region and click “Review + create”
![res_gr2](https://github.com/perseptron/cv/assets/30828895/ae01d62c-e908-43e8-9ef7-9a0fd3664ca1)

Click create in the next window

Now, we could create our web application using Azure Static Web Apps:
![web_app2-3](https://github.com/perseptron/cv/assets/30828895/c5bbf0ad-3177-45a1-8221-eea8e30adc46)

In the left menu of Azure Portal, navigate to Web and choose Static Web App  Create. 

Pick-up subscription and resource group in the next window.
Add a name to your app, then select Region for Azure Functions API. 
Select GitHub as source and login to it.
Choose project from your repository and select build preset (we are using clean html with styles so html is our choice) 
Click review + create, review our configuration and then click create on more time for start deploy process. 
After a few minutes (depend on source) we have our site up and ready.
![web_app4](https://github.com/perseptron/cv/assets/30828895/719812c1-614a-4d52-98a6-e1a2214534bc)

Click on url to visit it

Every time when we make new commits with our source and push it on remote, GitHub actions will trigger and redeploy all changes to our site.

Let’s check if it works. For that, find a heading tag in the index.html file and change it from 
`<h1><span>Louie Jie Mahusay</span></h1>`
 to 
`<h1><span>Agent Cooper</span></h1>`

Wait for a while then go to the web page and refresh it, we could see our changes
