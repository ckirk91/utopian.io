This is a fork of Utopian.io it was created with the intent to be used as a template for the front end of a STEEM blockchain based news website called Habari.io. This website will create a community that is similar to Utopian.io but for news content and not technichal content. Currently this version is just the fork of the utopian front end which our team is studying so we can begin designing the interface. Please feel free to reach out and help us with development! 
  
## Contributing to this Project
Get in touch on Discord: https://discord.gg/2B4sWyk

### Clone and Install
git clone https://github.com/utopian-io/utopian.io utopian.io

cd utopian.io

npm install

### Generate and Export SSL Certificates
openssl req -x509 -sha512 -newkey rsa:4096 -keyout key.pem -out cert.pem -days 365 -nodes

export SERVER_SSL_CERT="/path/cert.pem"

export SERVER_SSL_KEY="/path/key.pem"

export NODE_TLS_REJECT_UNAUTHORIZED=0

Replace path with the path to the generated .pem files.
You may need to authorise your browser in using a self-signed SSL certificate


### Set SC Utopian App
Add the enviroment variable UTOPIAN_APP using the app name of your Steem Connect oauth application. You can create a SC app here https://v2.steemconnect.com/apps/create. The same app will have to be used and setup in the backend https://github.com/utopian-io/api.utopian.io.

### Run The Frontend
npm run dev-server


#### API Server
Our sister project [utopian-io/api.utopian.io](https://github.com/utopian-io/api.utopian.io) provides the back-end APIs for Utopian. If you want to run Utopian locally, you **do need**  to run that project, though you may want to check it out!


## License
GNU Public License v3.0. Copyright Utopian.io

Original source code licensed under MIT License. Copyright Busy 
