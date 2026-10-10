# preview

Publishes a branch of [littlehammerlabs.com](https://github.com/Little-Hammer-Labs/littlehammerlabs.com) to **https://new.littlehammerlabs.com** for review before it goes to `main`. Search engines are told to stay out.

Redeploy after pushing to the branch:

```
gh workflow run deploy -R Little-Hammer-Labs/preview
gh workflow run deploy -R Little-Hammer-Labs/preview -f ref=some-other-branch
```

Which commit is live: https://new.littlehammerlabs.com/preview-ref.txt

DNS: Cloudflare CNAME `new` → `little-hammer-labs.github.io` (DNS only). Pages custom domain is set in this repo's settings.
