# Pi-hole
Running Pi-hole on docker


## Setup

Create a `.env` file at project root according to `example.env` and edit as needed

Start container

    docker compose up -d

Navigate to [Pi-hole dashboard](http://127.0.0.1:80/admin) and login with you password

Configure as needed. Key settings:

- Upstream DNS Servers
- Interface settings => permit all origins
- Use DNSSEC (optional)

Add blocklists from [here](https://v.firebog.net/hosts/lists.php) (optional)

Set client to use Pi-hole as their dns
