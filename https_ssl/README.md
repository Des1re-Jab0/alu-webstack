# HTTPS SSL

Securing web traffic with SSL termination on HAProxy.

- `0-world_wide_web`: Bash script (dig + awk) that audits the www, lb-01, web-01 and web-02 subdomains.
- `1-haproxy_ssl_termination`: HAProxy config terminating SSL on port 443 with a certbot certificate.
- `2-redirect_http_to_https`: HAProxy config that redirects HTTP to HTTPS with a 301.
