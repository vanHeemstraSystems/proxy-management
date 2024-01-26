proxy-management
# Proxy Management

A template for a microservice.

Can be read as "Proxy Management" at https://app.gitbook.com/???/????/

Can be browsed as "Proxy Management" at https://vanheemstrasystems.github.io/proxy-management/

Documentation of this repository is automatically done with Quarto using GitHub Actions

Based on "NGinX Proxy Manager" at https://nginxproxymanager.com/

Based on "Awesome Quarto" at https://github.com/mcanouil/awesome-quarto

Based on "Quarto Web" at https://github.com/quarto-dev/quarto-web and https://quarto.org/

Based on "Creating your personal website using Quarto" at https://ucsb-meds.github.io/creating-quarto-websites/

Based on "NGRok" at https://github.vanHeemstraSystems/ngrok

Create yarn.lock file as follows:

```
$ cd containers/app/main
$ yarn install
```

Run as follows:

```
$ cd containers/app
$ docker-compose --file docker-compose.dev.yml --project-name proxy-management-dev up --build -d
```
