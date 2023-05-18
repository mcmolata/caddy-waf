# caddy-waf
Waf based on caddy2

take it all in your Caddyfile
example
```
   route {
        waf {
            args_rule /etc/caddy/rules/args.rule
            user_agent_rule /etc/caddy/rules/user_agent.rule
            post_rule /etc/caddy/rules/post.rule
            ip_allow_rule /etc/caddy/rules/ip_allow.rule
            ip_block_rule /etc/caddy/rules/ip_block.rule
            rate_limit_bucket 10
            rate_limit_rate 10
        }
    }
```
