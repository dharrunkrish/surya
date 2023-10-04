 function src="https://smtpjs.com/v3/smtp.js"
        function sendemail(){
          Email.send({
            Host : "smtp.gmail.com",
            Username : "dharrunkri@gmail.com",
            Password : "youremailpassword",
            To : 'dharrunkri@gmail.com',
            From : document.getElementById("email").value,
            Subject : "New Contact From Enquiry",
            Body : "Name:"+document.getElementById("name").value+
                  "<br> Email:"+document.getElementById("email").value+
                  "<br> Subject:"+document.getElementById("subject").valuea+
                  "<br> Message:"+document.getElementById("message").value+
          }).then(
          message => alert("Message send successful")
          );
        }
