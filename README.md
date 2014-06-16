# Access My Info
Access my Info (AMI) is a web application that helps people to create justified requests for copies of their personal information from service providers. AMI is a step-by-step wizard that results in the generation of a personalized formal letter requesting access to the information a provider stores and utilizes about a person. The letter can be saved as a PDF, printed, and mailed through the post, or where available, directly emailed to a company’s privacy officer.

To start with, the application is focused on the PIPEDA framework for requesting access to personal information. This law forms the basis of the formal request. The longer term goal of AMI is to expand this functionality to accommodate requests justified under different laws or contracts around the world. Please contact Andrew Hilts if you are interested in contributing to the project.

The application is powered by JavaScript and runs entirely within the browser, including the creation of the PDF letter. It is designed so that no personal information is ever sent to the server. It is built using [Angular JS](https://angularjs.org/), [Bootstrap](http://getbootstrap.com/), [JSPDF](http://parall.ax/products/jspdf), [Font Awesome](http://fontawesome.io/), [Yeoman](http://yeoman.io/).

## Set up
To set up AMI for development on your system:

1. Ensure that you have all dependencies installed. You will need to install [Yeoman](http://yeoman.io/), [grunt](http://gruntjs.com/getting-started), [bower](http://bower.io/), and their dependencies ([node.js & npm](http://nodejs.org/) primarily). If you do not have them installed, install them later on in the process.

  - Install Node.js
    - type `git clone https://github.com/joyent/node.git`
      - then `cd node`
    - compile and install Node like this:
      - './configure'
      - 'make'
      - 'sudo make install'
    - check if node was installed correctly:
      - node -v

Install NPM

    Run the NPM install script:
        curl https://www.npmjs.org/install.sh | sudo sh
        And then check it works
            npm -v

Install Yeoman

    npm install -g yo

Install Grunt

    npm install -g grunt-cli

Install Bower

    npm install -g bower





2. In a terminal, Clone the repository and navigate into the root directory. 
    - open a terminal
    - make sure you're in your home directory `cd ~`
    - type `git clone https://github.com/bernardATdiymut/ami.git`


    git clone https://github.com/digitalstewards/ami.git
    cd ami
    Install bower requirements
        bower install



3. Still in the ami/ directory, to install the node components needed for the build environment
    - `npm install`

1. Then, run `grunt serve` to get a live development server running at localhost:9000
1. Open up the app source code in your text editor of choice. Most editing will need to be done within the `app/` directory
1. Once a file is saved, the server will reload the app in your browser, and changes can be previewed.

## Deployment
1. Once you want to take the app to production, run `grunt build` from the app root directory
1. This will create / update the `dist/` directory, which is a production-ready compilation of the app.
1. Navigate to the `dist/` directory and set up a git remote server to push to or simply upload the directory via FTP or your method of choice.

## License
Copyright 2014 Digital Stewardship Initiative Contributors (University of Toronto and Fort Effect Company Corporation)

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this software except in compliance with the License. You may obtain a copy of the License at:

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
