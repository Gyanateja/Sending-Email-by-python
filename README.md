import smtplib 
senderemail="kokkulteja@gmail.com"
reiceveremail="gyanakokkula@gmail.com"
password=input(str("please enter your password"))
message="Sending email by python"
server=smtplib.SMTP('smtp.gmail.com',587)
server.starttls()
server.login(senderemail,password)
print("------login success-----")
server.sendmail(senderemail,revemail,message)
print("message has been sent to",revemail)
