# check_link_checker

[gaurav-nelson/github-action-markdown-link-check@v1](https://github.com/gaurav-nelson/github-action-markdown-link-check)
is my favorite broken links detecting GitHub Action.

However, sometimes it does not seem to work.
Up until now, this has always been my fault.

This repo allows me to check myself in a simpler context.

## How to test the link checker.

There is a script that checks the link checker.

Modify `mlc_config.json` by removing the comma in line 6:

```
{
  "aliveStatusCodes": [200, 403, 418, 500, 503],
  "ignorePatterns": [
    {
      "pattern": "github/workspace/docs/software/overview$"
    },
    {
      "pattern": "http://hostname:8888"
    }
  ]
}
```

Now, the spell checker does not work anymore. This should be detected.

## Broken link

Here are broken links, to check the link checker:

[Broken link to website](https://absentwebsite.com/)
