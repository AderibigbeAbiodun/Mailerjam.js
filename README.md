# Mailerjam.js
Mailerjam.js is a javascript library that allow front-end developers to send email directly from javascript without the back-end code. 

<h2>Installation</h2>

* Download <a href="https://raw.githubusercontent.com/AderibigbeAbiodun/Mailerjam.js/cebc8a22873260ba199e1d77c3b4603d32ca30bf/maillerjam.js" download>Mailerjam.js</a>
* CDN link https://raw.githubusercontent.com/AderibigbeAbiodun/Mailerjam.js/cebc8a22873260ba199e1d77c3b4603d32ca30bf/maillerjam.js
* Generate <a href="">API Key</a>

<h2>Request function</h2>

	mailerjam({
		mailbody: {
			sender: "your-mail@exmaple.com", 	            // Sender Email
			to: "other-mail@exmaple.com", 	             // Receiver Email
			title: "MailerJam", 				                 // Title
			subject: "I am using mailerjam.js",		      // Subject
			body: "Send by mailerjam.js",			         // Message
		},
		smtp:{
			host: "exmaple.com",				          // Host
			username: "mail@exmaple.com",	        // Username
			password: "12345",			             // Password
		},
		api:{
			username: "Abbey",					 //Api Username
			apiKey: "xxxxx-xxxxx-xxxxx-xxxxx-xxxxx-xxxxx-xxxxx-xxxxx" // Mailerjam Api Key
		},
		success: function(response){
			console.log(response);
		}
	});
  
  <h2>Response Function</h2>
  
    success: function(response){
        console.log(response);
    }
    
  <h2>Response Callback Status</h2>

    200 - Mailer sent successfully
    400 - Failed due to some reason
    401 - Invalid API Key
    402 - Invalid API Username
    
<i>Note:</i> Mailerjam.js only work with secure email sever (SSL) base SMTP


Developed by Aderibigbe Abiodun
