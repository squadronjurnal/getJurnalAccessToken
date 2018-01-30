# getJurnalAccessToken
Register your app (https://developer.jurnal.id) & Create an App 
Or you can visit the full step here: https://api-jurnal.api-docs.io/v1/integration/public-integration

Then Development from your side to get access_token:

1. Setup Localhost 
*For this example i am using apache to connect my localhost

$ apachectl start

2. Use this code to get access token and put into index.html

$ git clone https://github.com/squadronjurnal/getJurnalAccessToken

3. Download https://ngrok.io and Setup HTTPS tunnel (Jurnal required HTTPS for your APP URL)
Run ngrok

$ ./ngrok http 80
You will find this after running ngrok:

For example https://624xxx.ngrok.io pointing to localhost:80 (which is your localhost)

4. Copy and paste your ngrok url (https) to developer.jurnal.id -> App URL 
After you update, install the app and open it 
Here, you already got jurnal access token and you will be able to connect to jurnal api depends on your scope when create your app
	
For example I want to post a transaction: sales invoice to my company 

5. Visit https://api-jurnal.api-docs.io and goto section Sales Invoice 
Use postman to test GET / POST / PATCH / DELETE by using base_url
https://api.jurnal.id/partner/core/api/v1/products
https://sandbox.jurnal.id/partner/core/api/v1/sales_invoices

Thank You :)


