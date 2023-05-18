# caddy-waf
Waf based on caddy2

take it all in your Caddyfile
example
```
   route {
        waf {
            args_rule args.rule
            user_agent_rule user_agent.rule
            post_rule post.rule
            ip_allow_rule ip_allow.rule
            ip_block_rule ip_block.rule
            rate_limit_bucket 10
            rate_limit_rate 10
        }
    }
```
