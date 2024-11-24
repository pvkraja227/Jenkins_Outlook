https://www.youtube.com/watch?v=HSu3PIilEV8

take ec2 (t2.med)
sudo apt update
install java17
install jenkins

check: outlook.com/settings/email/forwarding and IMAP/make sure POP and IMAP are enabled
https://account.microsoft.com/
security/turn on 2 step verification/create new app-pwd
get app-pwd (copy)

Jenkins Dashboard:

manage jenkins/install plugins/available plugins - stage view (make sure in installed plugins - Email Extension Plugin)
manage jenkins/system/
Extended E-mail Notification:
smtp.office365.com/587/use TLS/add credentials (username n pwd)
pvk23.ra@outlook.com / app-pwd (paste)/email-cred/email-cred
Default user e-mail suffix: @outlook.com
Reply To List: pvk23.ra@outlook.com
Default Triggers: Always

E-mail Notification:
smtp.office365.com/@outlook.com/use TLS/587
Use SMTP Authentication: pvk23.ra@outlook.com/app-pwd
Reply-To Address: pvk23.ra@outlook.com
Apply

new item/100/pipeline
buildnow
