# unraid-templates

[Unraid Community Applications](https://unraid.net/community/apps) templates for [SolidPing](https://solidping.io), self-hostable uptime monitoring.

- `templates/solidping.xml`: runs `ghcr.io/fclairamb/solidping` on port 4000, data in `/mnt/user/appdata/solidping`, as `nobody:users`.

Set `JWT secret` to a random string (`openssl rand -hex 32`). First login is `admin@solidping.io` / `solidpass`, changed on first use.

ICMP (ping) checks may need root: remove `--user 99:100` from Extra Parameters if you use them.

Support: https://github.com/fclairamb/solidping/issues
