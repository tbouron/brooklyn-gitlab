# brooklyn-gitlab

Pure Brooklyn YAML blueprint to deploy a [Gitlab](https://about.gitlab.com/) instance from the sources. This will
provision 3 VMs to deploy:

- a Redis store
- a PostgreSQL server
- a Gitlab instance with Nginx web server

Currently you can customize the following configuration:

- **gitlab.version**: The gitlab version you want to pull from the GIT repository (default: 7-11-stable)
- **gitlab.email.from**: The email address used to send notification emails (default: gitlab@brooklyn.local)
- **gitlab.email.display_name**: The email name (default: GitLab powered by Brooklyn)
- **gitlab.email.reply_to**: The email address to reply to (default: gitlab@brooklyn.local)
- **gitlab.db.username**: The DB username (default: git) 
- **gitlab.db.password**: The DB password (default: password)
- **gitlab.db.database**: The DB name (default: gitlabhq_production)