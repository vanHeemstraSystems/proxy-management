# NGinX Proxy Manager

Based on "NGinX Proxy Manager" at https://nginxproxymanager.com/

## How to setup the Nginx Proxy Manager

Based on "How to setup the Nginx Proxy Manager" at https://www.theserverside.com/blog/Coffee-Talk-Java-News-Stories-and-Opinions/How-to-setup-the-Nginx-Proxy-Manager-example

## Logging In

When your docker container is running, connect to it on port 81 for the admin interface. Sometimes this can take a little bit because of the entropy of keys.

```
http://127.0.0.1:81
```

Default Admin User:

```
Email:    admin@example.com
Password: changeme
```

Immediately after logging in with this default user you will be asked to modify your details and change your password.

## How to setup a reverse proxy with the Proxy Manager

Based on "How to setup the Nginx Proxy Manager" at https://www.theserverside.com/blog/Coffee-Talk-Java-News-Stories-and-Opinions/How-to-setup-the-Nginx-Proxy-Manager-example

To setup a reverse proxy with the Nginx Proxy Manager, simply click on the ‘Proxy Hosts’ link on the admin console’s dashboard and click the ‘Add Proxy Hosts’ button.

In the ‘Edit Proxy Host’ form that appears, simply fill out the domain name associated with the reverse proxy request, the IP address and the port number of the backend server to handle the request and click ‘Save.’

For example, we want the service "Main" to be proxied. Therefore we enter the following configuration:

- Domain Names: **localhost**

- Scheme: **http**

- Forward Hostname / IP: **<Hostname e.g. 'microservices.my-company.com'>**

- Forward Port: **4039**

- Cache Assets: **Yes**

- Block Common Exploits: **Yes**

- Websocket Support: **No**

- Access List: **Publicly Accessible**

As soon as the save button is clicked, the Nginx Proxy Manager activates the reverse proxy.

## Nginx Proxy Manager custom location settings

Based on "How to setup the Nginx Proxy Manager" at https://www.theserverside.com/blog/Coffee-Talk-Java-News-Stories-and-Opinions/How-to-setup-the-Nginx-Proxy-Manager-example


