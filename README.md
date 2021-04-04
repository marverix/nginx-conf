# Nginx Configuration

Security-focused Nginx Configuration based on OWASP recommendations 

## Sources

* [OWASP Application Security Verification Standard 4.0.2](https://raw.githubusercontent.com/OWASP/ASVS/master/4.0/OWASP%20Application%20Security%20Verification%20Standard%204.0.2-en.pdf)
* [OWASP Transport Layer Protection Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Transport_Layer_Protection_Cheat_Sheet.html)
* [Mozilla MDN Web Docs - HTTP Headers](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers)
* [Mozilla Web Security Cheat Sheet](https://infosec.mozilla.org/guidelines/web_security)
* [Mozilla SSL Configuration Generator](https://ssl-config.mozilla.org/)
* [Nginx Documentation](https://nginx.org/en/docs/)

## Usage

### nginx.conf

Each version is tagged, so you can basicly do something like this:

```sh
curl https://raw.githubusercontent.com/marverix/nginx-conf/TAG_HERE/nginx.conf > /etc/nginx/nginx.conf
```

Example for `v3`:

```sh
curl https://raw.githubusercontent.com/marverix/nginx-conf/v3/nginx.conf > /etc/nginx/nginx.conf
```

Or if you want always the latest version, use tag `latest`:

```sh
curl https://raw.githubusercontent.com/marverix/nginx-conf/latest/nginx.conf > /etc/nginx/nginx.conf
```

### mysite.conf

The same situation here:

```sh
curl https://raw.githubusercontent.com/marverix/nginx-conf/latest/mysite.conf > /etc/nginx/sites-available/your-site-name
```

Then enable:

```sh
ln -s /etc/nginx/sites-available/your-site-name /etc/nginx/sites-enabled/your-site-name
```

## License

Repo is under [ISC License](https://tldrlegal.com/license/-isc-license), so "basically, you can do whatever you want as long as you include the original copyright".

I didn't want to force anyone to share your patches, however I would be really grateful if you could help me co-create this config and share your improvements.

Thank you!
